---
share: true
created: 2023-05-26T14:51
updated: 2025-12-22T17:32
---

> [!info ] [Tại sao lại cần tải kho về hơn là đọc trên web?](./T%E1%BA%A1i%20sao%20l%E1%BA%A1i%20c%E1%BA%A7n%20t%E1%BA%A3i%20kho%20v%E1%BB%81%20h%C6%A1n%20l%C3%A0%20%C4%91%E1%BB%8Dc%20tr%C3%AAn%20web.md)

## Cài đặt tự động
Bộ cài này dành cho Windows 10 trở lên:

[Tải bộ cài :octicons-download-16:](https://Obsidian.Quảcầu.cc/assets/Obsidian, quản lý dự án và công cụ nghĩ.exe){ .md-button .md-button--primary }

Hình ảnh bộ cài:
![](https://i.imgur.com/e3iB6N3l.png)

Hình ảnh sau khi cài xong:
![](https://i.imgur.com/c6PDsL1.png)

Để đảm bảo an toàn cho máy bạn, Obsidian sẽ hỏi là bạn có muốn tin kho dữ liệu này không không. Hãy bấm *Trust author and enable plugins*. Obsidian sẽ bật Settings lên để bạn duyệt các plugin. Bạn có thể bấm vào *Check for updates* để cập nhật chúng, hoặc tắt đi cũng được:
![](https://i.imgur.com/MhgGMBc.png) 

Vậy là xong. 

Xem thêm:: [Các trục trặc có thể gặp khi cài](../3%20Th%C3%A0nh%20ph%E1%BA%A9m/Ph%E1%BA%A7n%20m%E1%BB%81m/B%E1%BB%99%20c%C3%A0i/C%C3%A1c%20tr%E1%BB%A5c%20tr%E1%BA%B7c%20c%C3%B3%20th%E1%BB%83%20g%E1%BA%B7p%20khi%20c%C3%A0i.md) 

## Cài đặt thủ công
### B1. Mở PowerShell với quyền admin
Bấm <kbd>Win+X</kbd> và chọn `Windows PowerShell (Terminal)`
![](https://st.quantrimang.com/photos/image/2018/07/09/cach-mo-powershell-nang-cao-trong-windows-10-5.jpg) 

### B2. Nhập lần lượt các lệnh sau
```PowerShell
New-ItemProperty -Path "HKLM:\SYSTEM\CurrentControlSet\Control\FileSystem" -Name "LongPathsEnabled" -Value 1 -PropertyType DWORD -Force
Set-Location "D:\" 
git config --global core.quotePath false
git config --global core.longpaths true
git config --global core.autocrlf true
git config --global core.safecrlf false
git clone https://github.com/QuaCau-TheSphere/quan-ly-du-an-va-cong-cu-nghi
Rename-Item "quan-ly-du-an-va-cong-cu-nghi/" "Obsidian, quản lý dự án và công cụ nghĩ"
git config --global --add safe.directory *
```

Nếu bạn chưa hiểu Git là gì nhưng cũng muốn thử sức thì có thể bắt đầu tìm hiểu ở bài [4 Du hành thời gian với Git](../../../%E2%9A%94%EF%B8%8F%20H%C6%B0%E1%BB%9Bng%20d%E1%BA%ABn%20Obsidian%20v%C3%A0%20Git/4%20Du%20h%C3%A0nh%20th%E1%BB%9Di%20gian%20v%E1%BB%9Bi%20Git/index.md)
