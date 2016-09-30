# **MARKDOWN**

> *Nội dung stask:*
> - Tìm hiểu cách sử dụng markdown
> - Các công cụ editor

#Mục lục:
[1. Tìm hiểu Markdown](#1)
 * [a/ Markdown là gì?](#1a)
 * [b/ Cú pháp cơ bản](#1b)
  * [Tiêu đề](#Tiêu-đề)
  * [Định dạng](#Định-dạng)
  * [Nhấn mạnh](#Nhấn-mạnh)
  * [Liên kết](#Liên-kết)
  * [Hình ảnh](#Hình-ảnh)
  * [Danh sách](#Danh-sách)
  * [Bảng](#Bảng)
  

[2. Cài đặt Sublime Text trên Ubuntu](#2)
 * [Giới thiệu Sublime text](#2a)
 * [Cài đặt](#2b)
 * [Cài đặt package control và plugin khác](#2c)
 

[3. Một số Editor khác](#3)

-----
## 1. Tìm hiểu Markdown <a name="1"></a>
 - ### a/ Markdown là gì? <a name="1a"></a>
  - Markdown là một ngôn ngữ đánh dấu với cú pháp văn bản thô, được thiết kế để có thể dễ dàng chuyển thành HTML và nhiều định dạng khác sử dụng một công cụ cùng tên. Nó thường được dùng để tạo các tập tin readme, viết tin nhắn trên các diễn đàn, và tạo văn bản có định dạng bằng một trình biên tập văn bản thô.
- Tham khảo [vi.wiki](https://vi.wikipedia.org/wiki/Markdown)

 - ### b/ Cú pháp cơ bản <a name="1b"></a>
* *Tiêu đề* <a name="Tiêu-đề"></a>
 
#Header 1: #Header 1
##Header 2: ##Header 2
###Header 3: ###Header 3
####Header 4: ####Header 4
#####Header 5: #####Header 5
######Header 6: ######Header 6

*  *Định dạng* <a name="Định-dạng"></a>
 - **In đậm** `*In đậm*`
 - *In nghiêng* `**In nghiêng**`
* *Nhấn mạnh* <a name="Nhấn-mạnh"></a>

 ```
 `Nhấn mạnh chuỗi`
 ```
 
 ```
 ```Nhấn mạnh đoạn văn.```
 ```
 
* *Liên kết* <a name="Liên-kết"></a>

 - Liên kết tường mình: https://trello.com/ `https://trello.com/`
 
    <https://trello.com/> ```<https://trello.com/>```
 - Liên kết rút gọn: [github](https://github.com) `[github](https://github.com)`

* *Hình ảnh* <a name="Hình-ảnh"></a>

 - Sử dụng `![title] (link)`

* *Danh sách* <a name="Danh-sách"></a>
 * Danh sách thường
 ```
* Tiêu đề 1
  * Mục 1
  * Mục 2
* Tiêu đề 2
* Tiêu đề 3
```
* Tiêu đề 1
  * Mục 1
  * Mục 2
* Tiêu đề 2
* Tiêu đề 3

 * Danh sách kiểu số
 
 ```
  1. Tiêu đề 1
   * Mục 1
   * Mục 2
  2. Tiêu đề 2
  3. Tiêu đề 3
  ```
  
1. Tiêu đề 1
 * Mục 1
 * Mục 2
2. Tiêu đề 2
3. Tiêu đề 3
 
* *Bảng* <a name="Bảng"></a>

```
| Cột 1| Cột 2 | Cột 3|
|------|-------|------|
| a    | 2     | x    |
| b    | 3     | y    |
| c    | 4     | z    |
```

| Cột 1| Cột 2 | Cột 3|
|------|-------|------|
| a    | 2     | x    |
| b    | 3     | y    |
| c    | 4     | z    |



## 2. Cài đặt Sublime Text trên Ubuntu <a name="2"></a>
### Giới thiệu Sublime text <a name="2a"></a>

 - Sublime Text là một trình soạn thảo phổ biến dùng để code, đánh dấu hay ghi chú. Là một editor mạnh mẽ cho giới lập trình viên vì được hỗ trợ nhiều plugin đa dạng. Phiên bản mới nhất là sublime text 3
 
### Cài đặt <a name="2b"></a>

 * Tải gói từ [trang chủ](https://www.sublimetext.com/3)
  
  `sudo dpkg -i Downloads/sublime-text_build-3114_amd64.deb`
  
 * Install bằng terminal
 
 ```
$ sudo add-apt-repository ppa:webupd8team/sublime-text-3
$ sudo apt-get update
$ sudo apt-get install sublime-text-installer
```

### Cài đặt package control và plugin khác <a name="2c"></a>

 - Để có thể cài đặt những plugin khác chúng ta cần cài đặt 1 plugin đặc biệt `package control`
 
 ```
 import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
 ```

 - Copy đoạn code trên.
 - ```Ctrl + ` ``` sau đó `Ctrl + v` để cài đặt package.
 - `Ctrl + Shift + P` -> `Package Control: Install Package` -> `export HTML` Để cài đặt plugin export HTML.
 - Tương tự hãy cài đặt markdown preview.

## 3. Một số Editor khác <a name="3"></a>
### [StackEdit - Editor](https://stackedit.io/editor)
### [Markdown Editor](http://dillinger.io/)
### [Markdown Table](http://www.tablesgenerator.com/markdown_tables)
