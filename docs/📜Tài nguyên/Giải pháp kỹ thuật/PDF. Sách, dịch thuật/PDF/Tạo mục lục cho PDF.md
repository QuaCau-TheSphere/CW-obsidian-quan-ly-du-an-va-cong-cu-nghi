---
share: true
created: 2023-05-26T14:51
updated: 2025-12-22T17:32
---
## Khi xuất ở Word 
Việc tạo mục lục là tối quan trọng. Không có mục lục thì chỉ thấy cây mà không thấy rừng. Bản thân mục lục cũng là những bảng tóm tắt. Chính việc nhớ mục lục khiến ta có thể ứng biến với tình huống khác nhau. [Tinh túy của một cuốn sách chính là mục lục của nó](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/M%C3%B4i%20tr%C6%B0%E1%BB%9Dng%20ngh%C4%A9,%20nh%E1%BA%ADn%20th%E1%BB%A9c%20t%C4%83ng%20c%C6%B0%E1%BB%9Dng/%C4%90%E1%BB%8Dc%20v%C3%A0%20vi%E1%BA%BFt/Tinh%20t%C3%BAy%20c%E1%BB%A7a%20m%E1%BB%99t%20cu%E1%BB%91n%20s%C3%A1ch%20ch%C3%ADnh%20l%C3%A0%20m%E1%BB%A5c%20l%E1%BB%A5c%20c%E1%BB%A7a%20n%C3%B3.md)
![](https://i.imgur.com/pybO2se.png)

## Creating hierarchical bookmarks/table of content

Use [Jpdfbookmark](https://sourceforge.net/projects/jpdfbookmarks/).

### Step 1: Prepare the table of content

Save the TOC in a .txt file in this format:

```
Chapter 1. The Beginning/23
    Para 1.1 Child of The Beginning/25,FitWidth,96
        Para 1.1.1 Child of Child of The Beginning/26,FitHeight,43
Chapter 2. The Continue/30,TopLeft,120,42
    Para 2.1 Child of The Beginning/32,FitPage
```
You can [ORC the TOC](https://stackoverflow.com/q/49954707/3416774) and use regex to fix it.

### Step 2: Load that TOC

![Machine generated alternative text:
ile Edit View Tools Window Help
Select Text
Ctrl+Alt+T
Use System Clipboard Ctrl+AIt+C
Show On Open
Dump
Apply Page Offset
Options
Ctrl+Alt+D
Ctrl+Alt+L
Ctrl+Alt+O](https://i.imgur.com/n42DaEL.png)

### Step 3: Prepare for step 4

This sounds dumb, but if you miss it you will be frustrated and have to do it again. Expand all bookmarks (Ctrl + E), select all of them, then go to Tools → Apply Page Offset

![Machine generated alternative text:
File Edit View Tools Window Help
Select Text
Ctrl+AIt
Use System Clipboard Ctrl+AIt+C
Show On Open
Dump
Apply Page Offset
Options
1.4 Invariance in Geometr•,
I. 5 Dimensional Analysis
1.6 Eddington's äÉæMethod of
I. 7 Ideal Numbers—
1.8 Actual Infinity and the Axi(
2 Intuitve Theories of
3 Axiomatc Set Theory—
4 Axiomatc Generalizatons of the
5 Representatonal Theory of Mea:
6 Intrinsicness
7 Qualitatveness
8 and the Axiom
References
Index
Ctrl+AIt+D
Ctrl+AIt+L
Ctrl+Alt+O](https://i.imgur.com/COshVw9.png)

### Step 4: Apply page offset

This step should be self-explained. Don’t forget to save.

That’s it. You are done. For more information, you can read its [manual](http://jpdfbookmarks.altervista.org/InsertBookmarks.html#1_3_1). The program has command line mode and can work on Linux, Mac.

If there are non-Roman characters, be sure to use the same encoding when dumping and applying bookmarks.
