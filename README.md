# HTML based on UI

## UI

## Comment

- HTML comment: 

```html 
<!-- This is HTML comment -->
```

## Typography

- Headings elements
```html 
<h1> heading 1 </h1>
<h2> heading 2 </h2>
<h3> heading 3 </h3>
<h4> heading 4 </h4>
<h5> heading 5 </h5>
<h6> heading 6 </h6>
```
- Paragraph element
```html 
<p> paragraph </p>
```
- Formatting elements
```html 
<i> italic text </i>
<em> emphasized text </em>
<b> bold text </b>
<strong> strong text </strong>
<ins> inserted text </ins>
<del> deleted text </del>
<mark> highlighted text </mark>
<sub> subscript text </sub>
<sup> superscript text </sup>
<small>small text </small>
```
- Quotations and citation
```html 
<q> quotation </q>
<abbr title="description text"> abbreviation </abbr>
<blockquote cite="absolute url address"> blockquote </blockquote>
<address> address </address>
<cite> painting, statue and ...  </cite>
<bdo dir="rtl"> bi-directional text </bdo>
```
- Computer code
```html 
<kbd> keyboard input </kbd>
<code> computer code </code>
<var> variable </var>
<samp> sample output </samp>
<pre> preformatted text </pre>
```
- Hyperlink
```html 
<a href="url address" target="_blank"> hyperlink </a>
<a href="file url address" download="file-optional-name"> hyperlink </a>
```

## Figure

- Picture
```html 
<picture>
  <source media="(min-width: screen-size)" srcset="image address" />
  ...
  <img src="image address" />
</picture>
```
- Image
```html 
  <img src="image address" alt="image description" />
```
- Image map
```html 
<img src="image address" alt="image description" usemap="#name" />

<map name="name">
  <area shape="shape" coords="coords" alt="image description" href="url address" />
  ...
</map>
```

## Container

- Division element
```html 
<div> division </div>
```
- Semantic elements
```html 
<header> header </header>
<nav> navigation menu </nav>
<main> main </main>
<footer> footer </footer>
<aside> aside </aside>

<section> 
    <h1>title</h1> 
    <p>description</p> 
</section>

<section> 
    <header>
        <h1>title</h1>
    </header>
    <div>
        <p>description</p>
    </div>
    <footer>
        <span>author: ...</span>
        <span>date: ...</span>
    </footer>
</section>

<article> 
    <h1>title</h1> 
    <p>description</p> 
</article>

<article> 
        <header>
        <h1>title</h1>
    </header>
    <div>
        <p>description</p>
    </div>
    <footer>
        <span>author: ...</span>
        <span>date: ...</span>
    </footer> 
</article>

<figure>
   <img src="url address" alt="image description" >
   <figcaption> image caption </figcaption>
</figure>
<mark> highlighted text </mark>
<address> address or author information </address>
<ruby> 明日 <rp>(</rp><rt>Ashita</rt><rp>)</rp> </ruby>
```

## Table

```html 
<table> 
    <caption></caption>
    <thead>
        <tr>
            <th></th>
            <th></th>
            <th></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan="2"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td colspan="3"></td>
        </tr>
    </tfoot>
</table>
```

## List

- Ordered list
```html 
<ol>
    <li>list item</li>
    ...
</ol>
```
- Unordered list
```html 
<ul>
    <li>list item</li>
    ...
</ul>
```
- Description list
```html 
<dl>
    <dt>description title</dt>
    <dd>description definition</dd>
    ...
</dl>
```

## Form

- form
    ```html
    <form method="post" enctype="multipart/form-data">
        ...
    </form>
    ```
- label
    ```html
    <label for="id value"> text </label>
    ```
- Input: input
   - textbox/textfield
    ```html
    <input type="text" name="name" minlength="4" maxlength="8" size="10" required />
    <input type="search" name="query" />
    <input type="url" name="url" pattern="https://.*" size="64" required />
    <input type="password" name="password" minlength="8" pattern="[0-9a-fA-F]{4,8}" required />
    <input id="pin" type="password" inputmode="numeric" minlength="4" maxlength="8" size="8" />
    <input type="email" name="email" pattern=".+@example\.com" size="64" required />
    
    <input type="email" size="40" list="email-list" />
    <datalist id="email-list">
        <option value="email address"></option>
        ...
    </datalist>
    ```
   - numberbox
    ```html
    <input type="number" name="number-in-stock" min="0" max="250" />
    <input type="tel" name="phone" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}" required />
    ```
   - button
    ```html
    <input type="button" value="popup login form" />
    <input type="submit" value="submit" />
    <input type="reset" value="reset" />
    ```
   - radio button
    ```html
    <input type="radio" name="gender" value="unknown" />
    <input type="radio" name="gender" value="male" />
    <input type="radio" name="gender" value="female" />
    ```
   - checkbox
    ```html
    <input type="checkbox" name="wrestling" value="wrestling" />
    <input type="checkbox" name="gulf" value="gulf" />
    <input type="checkbox" name="football" value="football" />
    <input type="checkbox" name="coding" value="coding" />
    ```
   - file upload
    ```html
    <input type="file" name="avatar-image" accept="image/png, image/jpeg, image/jpg" />
    <input type="file" name="credential-voice" accept="audio/*" />
    <input type="file" name="credential-video" accept="video/*" />
    <input type="file" name="profile-image" accept="image/*" />
    <input type="file" id="document" accept=".doc,.docx,.xml,application/msword" />
    ```
   - color palette
    ```html
    <input type="color" name="text-color" />
    <input type="color" name="bg-color" />
    ```
   - hidden
    ```html
    <input type="hidden" name="id" value="10" />
    ```
   - image
   ```html
    <input type="image" alt="label" src="url address" />
   ```
   - datetime
    ```html
    <input type="date" name="trip-start" value="2018-07-22" min="2018-01-01" max="2018-12-31" />
    <input type="datetime-local" name="meeting-time" value="2018-06-12T19:30" min="2018-06-07T00:00" max="2018-06-14T00:00" />
    <input type="month" name="start" min="2018-03" value="2018-05" />
    <input type="time" name="time" min="09:00" max="18:00" required />
    <input type="week" name="week" min="2018-W18" max="2018-W26" required />
    ```
    - range
    ```html
    <input type="range" name="volume" min="0" max="100" value="20" step="10" />
    ```
- Button: button
    ```html
    <button type="button"> ... </button>
    <button type="submit"> ... </button>
    <button type="reset"> ... </button>
    ```
- Textarea: textarea
    ```html
    <textarea name="description" rows="4"></textarea>
    ```
- Dropdown/Combobox: dropdown: select, option, optgroup
    ```html
    <select name="cars">
        <optgroup label="Swedish Cars">
            <option value="volvo">Volvo</option>
            <option value="saab">Saab</option>
        </optgroup>
        <optgroup label="German Cars">
            <option value="mercedes">Mercedes</option>
            <option value="bmw">BMW</option>
            <option value="audi">Audi</option>
        </optgroup>
    </select>
    ```

## Graphic

- Canvas
```html
<canvas id="playground" width="200" height="100">
    Your browser does not support the HTML canvas tag.
</canvas>
```
```js
const c = document.querySelector("#playground");
const ctx = c.getContext("2d");
ctx.moveTo(0,0);
ctx.lineTo(200,100);
ctx.stroke();
```
- SVG

```html
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>
```

## Multimedia

- iframe
```html
<a id="name" href="url address"> ... </a>
<iframe src="url address" width="width" height="height" name="name">
    iframe not supported by the browser
</iframe>
```
- Video
```html
<video src="file url address" controls loop mute autoplay></video>

<video>
    <source src="path/fileName.mp4" type="video/mp4" />
    <source src="path/fileName.ogg" type="video/ogg" />
    <track src="fileName.vtt" kind="subtitles" srclang="en" label="English" />
    <track src="fileName.vtt" kind="subtitles" srclang="no" label="Norwegian" />
    ...
</video>
```
- Audio
```html
<audio src="file url address" controls loop mute autoplay></audio>

<audio>
    <source src="path/fileName.ogg" type="audio/ogg" />
    <source src="path/fileName.mp3" type="audio/mpeg" />
    ...
</audio>
```
- File: embed - object
```html
<object data="file url address" width="width" height="height">
    <embed type="media-type" src="file url address" width="width" height="height" />
</object>
```
## Miscellaneous
- Line break
```html
    <br />
```
- Horizontal rule
```html
    <hr />
```
- Head
```html
    <title>page title</title>
    <link rel="stylesheet" href="css url address" />
    <meta charset="UTF-8" />
    <meta name="keywords" content="keyword1, keyword2, ..." />
    <meta name="description" content="page description" />
    <meta name="author" content="page author" />
    <meta http-equiv="refresh" content="30;url=url address" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <base href="absolute url address" target="_blank" />
    <script> ... </script>
```
- Entities, symbols and emojis
```html
    &nbsp;	&#160;
    &lt;	&#60;
    &gt;	&#62;

    &forall;    &#8704;
    &#8383;

    &#128516;
```
- url code
```html
    scheme://prefix.domain:port/path/filename?queryString=queryStringValue#fragment
```
- Language codes
```html
    <html lang="en"></html>
```
[List of language codes](https://www.w3schools.com/tags/ref_language_codes.asp)
- Country codes
```html
    <html lang="en-US"></html>
```
[List of country codes](https://www.w3schools.com/tags/ref_country_codes.asp)
- HTTP message
```html
    404
    500  
```
[List of http message](https://www.w3schools.com/tags/ref_httpmessages.asp)
- HTTP methods
```html
    PUT
    POST
    PUT
    PATCH
    DELETE
    CONNECT
    TRACE  
```
[List of http methods](https://www.w3schools.com/tags/ref_httpmethods.asp)