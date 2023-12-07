### HTML CSS HANDBOOK WITH PHUQUOCCHAMP

#### COURSES LINK

- Udemy
- Youtube
- [web.dev](https://web.dev/learn/html/welcome?continue=https%3A%2F%2Fweb.dev%2Flearn%2Fhtml%23article-https%3A%2F%2Fweb.dev%2Flearn%2Fhtml%2Fwelcome)

#### HTML CONTENT

##### 1. OVERVIEW

HTML (HyperText Markup Language) là một ngôn ngữ đánh dấu siêu văn bản dùng để mô tả cấu trúc của trang web. HTML bao gồm tâp hợp của các element và attribute được sử dụng để đánh dấu (mark up) tất cả components (thành phần) của tài liệu nhằm cấu trúc nó một cách ý nghĩa.

HTML document về cơ bản là tree of node bao gồm :

- HTML element.
- text node.

###### Element

HTML bao gồm tập hợp của nhiều element. Cấu trúc của một thẻ

![1701877442237](image/README/1701877442237.png)

###### Attribute

![1701877837508](image/README/1701877837508.png)

##### 2. DOCUMENT STRUCTURE

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
  
</body>
</html>
```

Thẻ `<html>` là một root element bao gồm nhiều thẻ bên trong (document head và document body)

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
```

Thẻ head không được nhìn thấy trên giao diện website nhưng nó lại có vai trò trong việc làm cho trang web hoạt động. Nó bao gồm :

- meta inforamation.
- search engines
- icon, font ...
- ....

###### !DOCTYPE html

Dùng để browser xác định mode để sử dụng (standard mode) để render, nếu không khai báo `!DOCTYPE html>` thì browser sẽ sử dụng mode khác để render trang web ([quirks mode](https://developer.mozilla.org/en-US/docs/Web/HTML/Quirks_Mode_and_Standards_Mode))

> Những trang web ngày xưa, các trang web được viết bằng 2 version
>
> - Netscape Navigator.
> - Microsoft Internet Explorer.
>
> Khi xuất hiện các qui chuẩn mới (W3C) thì ta không thể sử dụng chuẩn cũ này nữa nên người ta sử dụng DOCTYPE để định nghĩa chuẩn render được sử dụng.
>
> Có các chuẩn như :
>
> - quirks mode.
> - limited-quirks mode
> - no-quirks mode.

###### html

là một root element bao gồm 2 thẻ lớn `<head>` và `<body>` . Nếu như ta bỏ qua thì nó sẽ tự ngầm định, nhưng ta buộc phải khai báo nó vì nó định nghĩa ngôn ngữ, ....


**Content language**

```html
<html lang="en">
```

khai báo language attribute cho thẻ html sẽ giúp cho phép trình đọc màn hình, công cụ tìm kiếm và dịch thuật biết ngôn ngữ mà trang web đang sử dụng.

Ngoài ra ta cũng có thể sử dụng attribute "lang" để xác định một ngoại lệ ngôn ngữ được sử dụng trong trang web.

```html
<span lang="fr-fr">Ceci n'est pas une pipe.</span>
```
