---
share: true
created: 2023-05-26T14:51
updated: 2025-12-22T17:32
---
[PowerShell là một ngôn ngữ shell](PowerShell%20l%C3%A0%20m%E1%BB%99t%20ng%C3%B4n%20ng%E1%BB%AF%20shell.md)
[The Complete Guide to PowerShell Punctuation - Simple Talk](https://www.red-gate.com/simple-talk/sysadmin/powershell/the-complete-guide-to-powershell-punctuation/)
# Tạo nhiều folder
```PowerShell
$list=(ls -name -directory).substring(1)
foreach ($i in $list) {
	$index=$i.substring(0,1)
	cd "2$i" 
	new-item "2$index`1 Thành quả cần có" -type directory;
	new-item "2$index`2 Sự kiện" -type directory;
	new-item "2$index`3 Tài liệu" -type directory;
	Cd ..
}
```
# Tạo array
```PowerShell
$list|ForEach-Object {"`"$_`"," } |clip
```
# Đổi tên hàng loạt
```PowerShell
Get-ChildItem *.md, *.json -recurse | Where-Object {$_.name -cmatch '^2[A-Z]'}  | Rename-Item -newname { $_.name -replace '^2(.*)', '4$1'} -whatif 
```
- `-cmatch`: match có case sensitive
# Tìm và thay chuỗi hàng loạt
[VS Code nhiều khi không tìm hết được do tên file dài quá](VS%20Code%20nhi%E1%BB%81u%20khi%20kh%C3%B4ng%20t%C3%ACm%20h%E1%BA%BFt%20%C4%91%C6%B0%E1%BB%A3c%20do%20t%C3%AAn%20file%20d%C3%A0i%20qu%C3%A1.md)
```PowerShell
Get-ChildItem *.md, *.json -recurse | ForEach-Object { (Get-Content $_).Replace('Kết quả cần có::','Thành quả cần có::') | Set-Content $_ } 
```
# Xoá tất cả desktop.ini 
```PowerShell
Get-ChildItem -Force -Recurse -File -Filter "desktop.ini" | Remove-Item -force
```
# Tắt giới hạn số ký tự tối đa cho đường dẫn
```PowerShell
New-ItemProperty -Path "HKLM:\SYSTEM\CurrentControlSet\Control\FileSystem" -Name "LongPathsEnabled" -Value 1 -PropertyType DWORD -Force
```
[Maximum Path Length Limitation - Win32 apps | Microsoft Learn](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation?tabs=powershell#enable-long-paths-in-windows-10-version-1607-and-later)

# Thêm [biến môi trường](Bi%E1%BA%BFn%20m%C3%B4i%20tr%C6%B0%E1%BB%9Dng%20gi%C3%BAp%20ta%20%C4%91i%E1%BB%81n%20nh%E1%BB%AFng%20gi%C3%A1%20tr%E1%BB%8B%20l%E1%BA%B7p%20%C4%91i%20l%E1%BA%B7p%20l%E1%BA%A1i%20nhanh%20h%C6%A1n.md) 
```PowerShell
[System.Environment]::SetEnvironmentVariable('ResourceGroup','AZ_Resource_Group', 'User')
$env:PATH += ";SomeRandomPath"
```
```PowerShell
[Environment]::SetEnvironmentVariable("Path",    [Environment]::GetEnvironmentVariable("Path", [EnvironmentVariableTarget]::Machine) + ";C:\bin", [EnvironmentVariableTarget]::Machine)
```
# sfd
```PowerShell
$sourcePath = “F:\New folder”  
$destinationPath = “E:\New folder”  
$files = Get-ChildItem -Path $sourcePath -Recurse -Filter “*.*”  
foreach($file in $files){  
	$sourcePathFile = $file.FullName  
	$destinationPathFile = $file.FullName.Replace($sourcePath, $destinationPath)  
	$exists = Test-Path $destinationPathFile  
	if(!$exists){  
	$dir = Split-Path -parent $destinationPathFile  
	if (!(Test-Path($dir))) { New-Item -ItemType directory -Path $dir }  
	Copy-Item -Path $sourcePathFile -Destination $destinationPathFile -Recurse -Force  
	}  
	else{  
		$isFile = Test-Path -Path $destinationPathFile -PathType Leaf  
	if(!$isFile){  
		Copy-Item -Path $sourcePathFile -Destination $destinationPathFile -Recurse -Force  
	}  
	}  
}
```
