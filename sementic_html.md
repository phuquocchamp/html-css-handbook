### SEMENTIC HTML

##### SEMANTIC HTML

HTML ngữ nghĩa (Semantic HTML) là việc sử dụng các thẻ HTML có ý nghĩa cụ thể và rõ ràng để mô tả nội dung và cấu trúc của trang web. Sử dụng HTML ngữ nghĩa giúp trình duyệt, các công cụ tìm kiếm và các công nghệ hỗ trợ (như đọc màn hình) hiểu rõ hơn về cấu trúc và ý nghĩa của trang, đồng thời cũng giúp làm cho mã nguồn trở nên dễ đọc và hiểu.

###### Header

Header tag dùng để đánh dấu phần đầu của trang web, thường bao gồm:

- main title
- logo
- navigation links
- elements xuất hiện nhiều trên các trang trong trang web của bạn (phần nav bar)

```html
<!-- Non-semantic header -->
<div class="header">
  <h1>My Site</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </nav>
</div>

<!-- Semantic header -->
<header>
  <h1>My Site</h1>
  <nav>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>
</header>
```

###### Navigation

`<nav>` tag dùng để đánh dấu section của trang web chứa navigation links. Điều này sẽ giúp cho người sử dụng và search engines nhận biết rằng phần này được dùng cho việc điều hướng.

```html
<!-- Non-semantic navigation -->
<divclass="navigation">
  <ahref="#">Home</a>
  <ahref="#">About</a>
  <ahref="#">Contact</a>
</div>

<!-- Semantic navigation -->
<nav>
  <ul>
    <li><ahref="#">Home</a></li>
    <li><ahref="#">About</a></li>
    <li><ahref="#">Contact</a></li>
  </ul>
</nav>
```

###### Main

Thẻ `<main> `  dùng để đánh dấu phần nội dung chính của trang web. Điều này giúp cho user và search engines xác định phần nội dung chính của trang web

```html
<!-- Non-semantic main content -->
<divclass="main-content">
  <h2>About Us</h2>
  <p>Welcome to our website. We are a company that specializes in widgets.</p>
</div>

<!-- Semantic main content -->
<main>
  <h2>About Us</h2>
  <p>Welcome to our website. We are a company that specializes in widgets.</p>
</main>
```

###### Article

Thẻ `<article>` dùng để đại diện cho phần nội dung độc lập, chẳng hặn như :

- blog post.
- news article
- product review

Nội dung trong thẻ `<article>` phải có ý nghĩa và có thể bao gồm các thẻ khác như :

- heading
- paragraph
- image
- other type of content.

```html
<!-- Non-semantic article -->
<divclass="article">
  <h2>How to Make a Widget</h2>
  <p>Widgets are great. Here's how to make one.</p>
</div>

<!-- Semantic article -->
<article>
  <h2>How to Make a Widget</h2>
  <p>Widgets are great. Here's how to make one.</p>
</article>
```

###### Aside

Thẻ `<aside>` được sử dụng để đánh dấu một phần của trang chứa thông tin không phải là nội dung chính của trang, thường là:

- thông tin bổ sung
- liên quan
- quảng cáo.

Thẻ `<aside>` có thể chứa các thành phần như:

- biểu đồ
- quảng cáo
- liên kết có liên quan
- hoặc bất kỳ nội dung phụ khác.

```html
<div>
  <article>
    <h2>Article Title</h2>
    <p>Article content goes here</p>
  </article>
  <aside>
    <h3>Related Articles</h3>
    <ul>
      <li><ahref="#">Article 1</a></li>
      <li><ahref="#">Article 2</a></li>
      <li><ahref="#">Article 3</a></li>
    </ul>
  </aside>
</div>
```

###### Section

Thẻ `<section>` dùng để đánh dấu các phần của trang web được nhóm theo chủ đề với nhau. Thẻ này thường bao gồm những nội dung như :

- Chương
- Phần

của một bài viết dài, hoặc các phần khác nhau của trang.

```html
<section>
  <h2>Section Title</h2>
  <p>Section content goes here</p>
</section>
```

###### Footer

Dùng để đánh dấu phần nội dung phía dưới của web page, như :

- copyright infomation.
- contact details
- links to social media profiles.

```html
<!-- Non-semantic footer -->
<divclass="footer">
  <p>© 2021 My Site</p>
</div>

<!-- Semantic footer -->
<footer>
  <p>© 2021 My Site</p>
</footer>
```

###### Details and Summary

The **details** and **summary** tags used to mark up a collaptible section of content. The `<summary>` tag is used to mark up the title of section, and the `<details> ` tag is used to mark up the content it self.

```html
<details>
    <summary>Click to expand</summary>
    <p> Content goes here </p>
</details>
```

###### Figure and Figcaption

The `<figure>` and `<figcaption>` tags are used to mark up a self-contained piece of content that is referenced from the main content of a web page. The `<figure>` tag is used to mark up the content itself, and the `<figcaption>` tag is used to mark up a caption or description for the content.

```html
<figure>
  <imgsrc="image.jpg"alt="Image description" />
  <figcaption>Image caption</figcaption>
</figure>
```

###### Mark

The `<mark>` tag is used to mark up text that has been highlighted for some reason. This might include things like search results, or text that has been highlighted by a user.

```html
<p>Here is some <mark>highlighted</mark> text.</p>
```

###### Time

The `<time>` tag is used to mark up a date or time. By using the `<time>` tag, you can make it easier for search engines and other technologies to understand the meaning of the content on your page.

###### Progress

The `<progress>` tag is used to mark up a progress bar. By using the `<progress>` tag, you can make it easier for users to understand the progress of a task.

```html
<progressvalue="50"max="100"></progress>
```

###### What about `<div>` and `<span>`?

The `<div>` and `<span>` tags are not semantic tags. They are used to mark up generic content areas, and do not convey any specific meaning. You should only use these tags if you have no other option.
