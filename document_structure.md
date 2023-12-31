
### DOCUMENT STRUCTURE

Cấu  trúc :

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

###### head

Character encoding được khai báo trong thẻ head dùng để cho browser render theo kiểu charset được khai báo .

```html
<meta charset="utf-8" />
```

###### Document title

Trang home page hoặc các trang còn lại cần nên có một title duy nhất.

###### Viewport metadata

Thẻ `<meta>` với thuộc tính `viewport` được sử dụng trong HTML để điều chỉnh cách mà trang web được hiển thị trên các thiết bị di động. Điều này đặc biệt quan trọng để làm cho trang web phản ánh đúng trên các màn hình kích thước khác nhau và tránh các vấn đề liên quan đến zoom hoặc cách trang web hiển thị trên các thiết bị di động.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

* `width=device-width`: Điều này nói với trình duyệt để thiết lập chiều rộng của trang bằng với chiều rộng của thiết bị di động.
* `initial-scale=1.0`: Điều này xác định mức độ phóng ban đầu của trang. Giá trị 1.0 đảm bảo rằng trang không được phóng to hoặc thu nhỏ khi tải lần đầu tiên.
