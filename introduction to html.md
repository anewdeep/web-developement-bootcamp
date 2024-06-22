# Getting started with HTML

## Core web technology

- Every website is built on HTML.
- HTML code is based on tags.
- Tags use angle brackets `<>`.
- Angle brackets surround the name of the element to be added to the webpage. Elements like button, text, and images, are added to webpages with different tags.
- `<img>` tag to add images to a webpage.

    `<button>, <img>, <p>, <table>`
- **HTML** is used to build the structure of a webpage.
- **CSS** styles a webpage.
- **Javascript** makes pages interactive.

## HTML code

- HTML code tells browser how to display a webpage.
- Many elements require both opening and closing tags.

    `<button>like</button>`
- Closing tags are similar to opening tags except they contain a slash `/`.
- Content of the button is placed between tags.
- Many elements require both opening and closing tags (also called **container tags**). Paragraph text is another example.

    `<p>Paragraph</p>`
- Multiple elements can be combined in a code.
- Web browser can read HTML code and translate it into a webpage.

## Headings

- Text on a webpage can be organized in different sections with headings.
- Headings also helps search engines know what a webpage is about, to show it to the right table.
- Headings in HTML comes in different levels.
- `<h1>` defines the most important heading.

    `<h1>Heading 1</h1>`
- 6 levels of headings in HTML `<h1>...<h6>`.
- Requires both opening and closing tags.
- Different headings can be added to organize content
- `<h1>` styled with largest font, `<h6>` is the smallest.
- Headings can be combined with other elements.
- <h1> is the most important heading. THere should only be one level 1 heading per page.
- Heading levels must be used in correct order.
- Some HTML elements can be defined with only one tag. They're called **empty tags**.
- `<img>` doesn't require a closing tag.

## Images

- webpages with images get more views, rank higher in search results, and get shared more on social media.
- `<img>` HTML tag is used for image element.
- Source of the image needs to be included in the tag.

    `<img src = "https://toppng.com/uploads/preview/html5-logo-11609363747dunzzmadxo.png" height = 100>`

    <img src = "https://toppng.com/uploads/preview/html5-logo-11609363747dunzzmadxo.png" height = 100>

- `src` is the location on the internet where image is stored.
- Web browsers request information from the web to put together and display webpages.
- Code, documents and media files such as images and videos put together byu the browser to display the resulting webpage.
- Web servers are computers that are always connected to the internet and continuously listen for info requests.
- URL is a location (address) on the web. Image URL needs to be enclosed in either single or double quotes.

    ```
        <h1>Heading text</h1>
        <p>Paragraph text</p>
        <img src = "https://toppng.com/uploads/preview/html5-logo-11609363747dunzzmadxo.png">
        <button>Button</button>
    ```
    <table>
        <tr>
            <td>
                &lt;h1&gt;Heading text&lt;/h1&gt;
            </td>
            <td>
                <h1>Heading text</h1>
            </td>
        </tr>
        <tr>
            <td>
                &lt;p&gt;Paragraph text&lt;/p&gt;
            </td>
            <td>
                <p>Paragraph text</p>
            </td>
        </tr>
        <tr>
            <td>
                &lt;img src = "https://toppng.com/uploads/preview/html5-logo-11609363747dunzzmadxo.png"&gt;Heading text&lt;/h1&gt;
            </td>
            <td>
                <img src = "https://toppng.com/uploads/preview/html5-logo-11609363747dunzzmadxo.png" height = 80>
            </td>
        </tr>
        <tr>
            <td>
                &lt;button&gt;nuke&lt;/button&gt;
            </td>
            <td>
                <button>nuke</button>
            </td>
        </tr>
    </table>

# Going deeper with HTML

## Comments

- Comments helps other users read your code.
- Can add notes and explanation to code with comment tags.

    `<!-- comment goes here-->`
- Ignored by browsers and not displayed on webpage.
- Can be used to temporarily disable part of a code so that it isn't displayed by the browser.
- HTML is case insensitive language. Browser will understand tags in both cases.
- Web browser ignores whitespace and line breaks in code.
- Line breaks in elements like paragraphs are ignored by the browser.

    ```
        <p>line 1
        line 2</p>
    ```
        <p>line 1
        line 2</p>
- `<br>` tag forces a **line break**.

    ```
        <p>line 1<br>
        line 2</p>
    ```
    <p>line 1<br>
    line 2</p>
- Elements like headings and paragraphs automatically start on new line when created.

## Standards and best practices

- Needed to make webpages compatible with different browsers and devices.
- Teamwork and collaboration are more effective.
- `<body>` container tag groups everything that gets displayed on a page when loaded in a browser.
- Body tags are needed for a page to be compatible with all web browsers.
- webpage can contain only one body element.
- Nesting: HTML tags inside other tags.
- `<head>` container tag includes technical information about a webpage.
- Increases visibility and traffic from search engines.
- Title, description, and keywords are nested inside the head tag.
- Head needs to be placed before the body.
- Information in the head is not displayed on the webpage. Only title is shown in search engines and browser tabs.
- `<html>` tags wrap html code. Head and body are nested inside html tags.
- Indentation- spaces at the beginning of lines- is considered a good practice to improve code readibility.
- Different levels of indentation used to show nesting.

## Text formatting

- Helps website visitors find the information they're looking for.
- Used to highlight important content on a page and make websites more accessible and inclusive.
- HTML **formatting tags** are used to change how text is displayed.
- `<b>` bold tag displays text in bold.

    `<b>Bold text</b>` ->
    <b>Bold text</b>
- Formatting tags are container tags.
- `<i>` italics tag displays text in italics.

    `<i>Italics text</i>` -> <i>Italics text</i>
- `<u>` underlines text

    `<u>underlined text</u>` -> <u>Underlined text</u>
- Formatting tags are applied to text and can be nested inside other elements.

    ```
        <p><b>bold</b></p>
        <p><i>italics</i></p>
        <p><u>underlined</u></p>
    ```
    <p><b>bold</b></p>
    <p><i>italics</i></p>
    <p><u>underlined</u></p>
- webpages are designed to be accessible by people with disabilities. Web accessibility is all about making websites more inclusive and removing barriers.
- **Screen readers** are programs that make content of a website accessible to users who are blind, visually impaired, or have a learning disability.
- `<strong>` used to highlight important text. Displayed in bold, but has a meaning and is used by screen readers.
- `<em>` used to define emphasized text. Displayed in italics but screen readers will verbally stress the word.
- `<strong>` and `<em>` are semantic formatting tags because they add meaning to the content.

## Links

- **HyperText**: lets people jump from one webpage to another through links. HyperText is a text that contains link to another page. webpages are called HyperText because they're connected by HyperTextlinks (or hyperlinks).
- **Hyperlinks**: allows users to move from one page to another and share information across different machines and systems.
- `<a>` anchor tag used to create hyperlink to a webpage. Is a container tag.
- `href`: adds destination url to create links. (HyperText reference)
- URL needs to be enclosed in matching quotes.
- Hyperlinks can be nested inside other text elements.
- Content of anchor tag is text that is to be displayed.
- Hyperlinks can also connect pages of the same website.
- Part of the URL that stays the same for all of a website's pages is the **domain name**.
- HTML stands for **HyperText Markup Language**.

    `<a href = "https://www.youtube.com">Broadcast Yourself</a>` -> <a href = "https://www.youtube.com">Broadcast Yourself</a>

## Lists

- Lists are very useful elements. Can be used to build navigation menus.
- List contains of list items `<li>`.
- Container tags.
- **Ordered lists**: shows numbers instead of bullet points. Used when order of list items is of importance.

    ```
        <ol>
            <li>one</li>
            <li>two</li>
            <li>three</li>
        </ol>
    ```

    <ol>
        <li>one</li>
        <li>two</li>
        <li>three</li>
    </ol>
- **Unordered lists**: shows bullet points. Used when order of the list items is not imporant.

    ```
        <ul>
            <li>bacon</li>
            <li>eggs</li>
            <li>bread</li>
        </ul>
    ```

    <ul>
        <li>bacon</li>
        <li>eggs</li>
        <li>bread</li>
    </ul>
- Lists can be nested.
- Each list item displayed on a new line.

# Using attributes

## Attributes

- Attributes give more control over HTML elements.
- Attributes are modifiers that provide additional information about elements.
- Attributes can be optional or required. For example, `<img>` requires an attribute to work.
- For container tags, attributes always go into the opening tag. For example, `href` attribute of the `<a>` tag.
- `alt` attribute describes what images are showing.

    `img src = "img.png" alt = "dark side of the moon"`
- `alt` attribute is read aloud by screen readers, shown when the image doesn't load, and read by search engines. This makes the page more accessible.
- Attributes come in name-value pairs.
- Image size can be controlled using `width` and `height` attribute, measured in pixels by default.
- Changing the aspect ratio between width and height, distorts the image.

    `<img src = "https://toppng.com/uploads/preview/html5-logo-11609363747dunzzmadxo.png" height = 80>`

    <img src = "https://toppng.com/uploads/preview/html5-logo-11609363747dunzzmadxo.png" height = "80" width = "100">

## Menu and navigation

- Websites come in 2 types: multiple page websites and single page websites.
- Multi-page websites are made of more than one page.
- Navigating between pages requires the web browser to load different HTML files.
- `<nav>` container tag defines a set of links that allows the user to naavigate between pages of a website.

    ```
        <nav>
            <a href = "https://www.youtube.com">Youtube</a>
            <a href = "https://www.twitch.tv">Twitch</a>
            <a href = "https://www.instagram.com">Instagram</a>
        </nav>
    ```

    <nav>
        <a href = "https://www.youtube.com">Youtube</a>
        <a href = "https://www.twitch.tv">Twitch</a>
        <a href = "https://www.instagram.com">Instagram</a>
    </nav>
- Links to different pages are added with the anchor tag and nested inside the nav container tag.
- html documents are saved with .html extension.
- A single page website has all its content on the home page. Any navigation links takes the user down to different sections instead of loading new pages.
- Best practice to name homepage `index.html` so that the browser can find and load it.
- To jump to a specific part of a single page website, sections must be marked with the `id` attribute.

    `<h2 id = "section-1">Section 1</h2>`
- `id` attribute is used to identify the element that are targeted as a navigation link.
- Each id attribute **must be unique** and with quotes.
- Once the element you want to jump to has been marked with the id attribute, it can be targeted with the anchor tag.

    `<a href = "#section-1">go to s1</a>`
- Hash (`#`) needed to tell the web browser, that we are targeting a section of the same page.
- `href = "#top"` takes user back to the top of a page.

## Forms

- Forms are used to interact with the visitors of a website and collect information from them.
- Forms can be used to: -
    - get in contact
    - send orders, requests and other information
    - create account or register
    - and much more
- Forms made up of input elements like text fields, checkboxes, and submit buttons. These input elements are nested inside the `<form>` container tag.

    ```
        <form>
            <!-- input elements go here>
        </form>
    ```
- The most common element is `<input>`. There are many forms of input element, depending on the `type` attribute.

    ```
        <input type = "text">
        <input type = "radio">
        <input type = "checkbox">
    ```
    <input type = "text"><br>
    <input type = "radio"><br>
    <input type = "checkbox">
- Form elements will be displayed on the same line unless `<br>` tag is used.
- Labels can be added for different input elements with the `<label>` tag.

    ```
        <form>
            <label>email: </label>
            <input type = "text">
        </form>
    ```
    <form>
        <label>email: </label>
        <input type = "text">
    </form>
- Label can be connected to the input elements with the use of `for` and `id` attributes.

    ```
        <form>
            <input type = "checkbox" id = "box1">
            <label for = "box1">Subsribe to newsletters</label><br>
            <input type = "checkbox" id = "box2">
            <label for = "box2">Receive promotional mails</label>
        </form>
    ```
    <form>
        <input type = "checkbox" id = "box1">
        <label for = "box1">Subsribe to newsletters</label><br>
        <input type = "checkbox" id = "box2">
        <label for = "box2">Receive promotional mails</label>
    </form>
- `id` attribute is used to identify a unique input element. `for` attribute in a label, targets and matches an input's id.
- Connecting labels and inputs, **increases the hit area**. Interacting with labels, selects the form field.

## Submitting forms

- HTML form is a convenient way to send data to a database hosted on a server.
- A submit button is used to send the data in a form. The submet type oof input, adds button to a form.

    `<input type = "submit">` -> <input type = "submit">
- The name attribute is used to reference the data after submitting the form.

    ```
        <input type = "text" name = "email">
        <input type = "text" name = "city">
        <input type = "submit">
    ```
- Only forms elements with a `name` attribute will have their values passed to the database when submitting a form.
- The `name` attribute is used to put the input from the user in the correct field (column) in the database.

    <center>
        <img src = "https://lecontent.sololearn.com/material-images/768cdbb978ff468ca7b70dfd65f94cfd-14A.png", height = "150">
    </center>
- `name` attribute is added to input fields.
- `value` attribute defines the value that is submitted when the input is selected.

    <input type = "radio" id = "r1" name = "pay" value = "cash">
    <label for = "r1">Cash</label>
    <input type = "radio" id = "r2" name = "pay" value = "card">
    <label for = "r2">Card</label>
- Names and values are needed to correctly store information in the database. HTML code needs to include where and what to put in the database.
- For text inputs, value attribute can be used to define a default value that will be submitted, unless a different value is provided by the user.

    ```
        <label for = "t1">Email: </label>
        <input type = "text" id = "t1" name = "email" value = "example@domain.com">
    ```

## Drop down menu

- Drop down menu makes form more efficient, accessible, and organized.
- `<select>` container tag used to create a drop down list.
- `<option>` container tag is used inside `<select>` to add choices.
- `value` attribute can be used to control what data each option sends to the database.
- `selected` attribute creates a drop down menu with pre-selected option. Pre selected option will be displayed first.
- Labels can be added to drop down menu.
- Lables and drop down menus are connected with the `for` and `id` attribute.

    ```
        <label for = "color-selection">Pick your favorite color: </label>
        <select id = "color-selection">
            <option value = "red">red</option>
            <option value = "green">green</option>
            <option value = "black" selected>black</option>
        </select>
    ```

    <label for = "color-selection">Pick your favorite color: </label>
    <select id = "color-selection">
        <option value = "red">red</option>
        <option value = "green">green</option>
        <option value = "black" selected>black</option>
    </select>
- Other types of input elements include `email`, `password`, `tel` etc.

# Mastering HTML

## Videos

- `<video>` container tag to embed video files into a webpage.
- Different video formats can be added. Common formats include mp4, ogg, webm.
- `<source>` empty tag provides the location and format of the video file.
- `src` attribute specifies url of the video file.
- `type` attribute specifies format of the video file.
- Different media formats are needed for compatibility with different browsers and devices.
- Source tag allows adding multiple files.
- When different `<source>` options are included, the browser will choose the first one it supports.
- Text can be added inside video tags. It will only be displayed in browsers that don't support the video element.
- `controls` attribute can be used to display play, pause, volume, and other controls.

    ```
        <video controls loop autoplay muted>
            <source src = "https://files.catbox.moe/umt2w0.webm"
                    type = "video/webm">
            video not supported
        </video>
    ```

    <video controls loop autoplay muted>
        <source src = "https://files.catbox.moe/umt2w0.webm"
                type = "video/webm">
        video not supported
    </video>

## Music and audio

- `<audio>` container tag to add audio.
- <source> tag adds source option for the audio.
- `src` attribute adds audio file's url.
- `type` attribute adds format.
- Common formats include mp3, wav, ogg.
- Can use `autoplay`, `muted`, and `loop` attributes to control the behaviour of the multimedia element.
- These attributes can be used with both audio and video elements.

## Page layout

- Layout of a webpage can improve user experience and make the content more readable.
- Body of a webpage can be divided into three parts: -
    1. **Header**: `<header>`
    2. **Main** content: `<main>`
    3. **Footer**: `<footer>`
- `<header>` tag contains introductory information.
- Several header elements can be added to a webpage.
    ```
        <header>
            <!-- intro -->
        </header>
    ```
- Contains navigation links, menu, and/or search bar.
- Brand elements like logos, are usually found in the header top.
- `<main>` container tag includes the main content of a webpage.
    ```
        <main>
            <!-- main elements -->
        </main>
    ```
- There must not be more than one main element.
- `<footer>` container tag contains contact, legal information, and links.
    ```
        <footer>
            <!-- footer information -->
        </footer>
    ```
- There can be several footers in a document.
- `<header>`, `<main>`, and `<footer>` elements are nested in the `<body>` container tag.
- **Responsive web design** makes webpages look great on any screen.
- Building a website invlolves 2 areas: -
    - **front-end**: what users see and interact with.
    - **back-end**: information requests, servers and databases.

## More on layout

- `<article>` represents an independent, self-contained piece of content.
- An article is content that would make sense on its own.

    ```
        <article>
            <h1>5 future-proof jobs</h1>
            <p>Coding</p>
        </article>
    ```
- Used for content like news stories and blog posts.
- Layout tags like header, main, footer, article etc. are **semantic tags** because they give information about what they contain.
- `<section>` helps break down content into parts.

    ```
        <section>
            <h2>About us</h2>
            <p>We are a small company.</p>
        </section>
    ```
- Semantic tag usually contains a heading.
- A webpage could be split into separte sections- for introduction, contact information etc.
- Section can be used to separate each chapter, news, item etc.
- `<aside>` used for secondary, additional, or related content.

    ```
        <aside>
            <h2>Related topics</h2>
            <p>More on HTML</p>
        </aside>
    ```
- These elements can be combined to create a well-structured semantic layout for content.

<img src = "https://lecontent.sololearn.com/material-images/74eba75ee884492bad9497b4c8a360bc-HTML4.4.13.png" height = 250 style="display: block; margin-left: auto; margin-right: auto;">

- Semantic tags don't give any visual effect to the content.
- Layout elements can be nested to create organized and accessible pages.

## The style attribute

- Fully customize the visual presentation of a website, from typography and colours, to layout and more.
- Changing colour of text with `style` attribute

    `<p style = "color:green">green</p>`
    <p style = "color:green">green</p>
- Style attribute can be used to define properties like colour, font size and alignment.
- Can customize multiple properties at the same time by separating each propert:value pair with a semi-colon.

    `<h1 style = "color:blue; text-align:center">centered blue text</h1>`
    <h1 style = "color:blue; text-align:center">centered blue text</h1>

- Font size can be changed with `font-size` property. `style = "font-size:large"`
- `background-color` property useful for styling elements like buttons.
- Some style properties require multiple values, like the `border` property.
    
    `<p style = "border:5px solid red; width:50px; height:25px">nuke</p>`
    <p style = "border:5px solid red; width:50px; height:25px">nuke</p>

- The only required border sub-property is border-style. If width not specified, default value is "medium". Color not specified, border colour will be the same as text colour.
- Border styles: dashed, dotted, double, inset, outset, solid.
- **CSS** makes website styling more efficient, consistent, and more in harmony.

## Inline and block element

- Block level elements always start on a new line.
- Inline elements don't start on a new line.
- Block level elements take up the full width available.
- Inline elements take as much width as necessary.
- Format tags are inline elements.
- Inline elements can be nested inside block level elements.
- Line break `<br>`, is used to force inline elements to start on a new line.

## Divide and conquer

- Grouping different HTML elements can make pages load faster and easier to customize and maintain.
- `<div>` element is a container for HTML elements that keeps pages organized.
- div element is block level element, takes up full width.
- Elements grouped in `<div>` can be styled quicker, all at once.
- div is a container that groups related content on a webpage, such as a sidebar, navigation menu etc.
- Doesn't add meaning to content because it's a non-semantic tag.
- The style in `<div>` will apply to all its nested elements unless you given them their own.

## Tables

- Helps display data in a way that's easy to scan, compare, and analyze.
- `<table>` container to add tables.
- Table data made of rows and columns.
- `<tr>` container tag to add rows to a table. Rows are nested in table tag.
- `<td>` (table data) to add cells. Nested in rows.

    ```
        <table style = "border: 2px solid; border-collapse: collapse;">
            <tr style = "border: 1px solid;">
                <th style = "border: 1px solid; padding:10px">Name</th>
                <th style = "border: 1px solid; padding:10px">Email</th>
            </tr>
            <tr>
                <td style = "border: 1px solid; padding:10px">John Doe</td>
                <td style = "border: 1px solid; padding:10px">johndoe@gmail.com</td>
            </tr>
            <tr>
                <td style = "border: 1px solid; padding:10px">Jane Doe</td>
                <td style = "border: 1px solid; padding:10px">janedoe@gmail.com</td>
            </tr>
        </table>
    ```

    <table style = "border: 2px solid; border-collapse: collapse;">
        <tr style = "border: 1px solid;">
            <th style = "border: 1px solid; padding:10px">Name</th>
            <th style = "border: 1px solid; padding:10px">Email</th>
        </tr>
        <tr>
            <td style = "border: 1px solid; padding:10px">John Doe</td>
            <td style = "border: 1px solid; padding:10px">johndoe@gmail.com</td>
        </tr>
        <tr>
            <td style = "border: 1px solid; padding:10px">Jane Doe</td>
            <td style = "border: 1px solid; padding:10px">janedoe@gmail.com</td>
        </tr>
    </table>

- Borders can be added to tables, rows, and cells with `style` attribute.
- Tables contain headers. Header is a special row at the top the the table used to label each column. `<th>` tag.
- Several headers can be included in HTML tables.
- Cells can take up multiple rows or cells using attributes `colspan` & `rowspan` (*merging cells*).
- `colspan`: no of columns a cell should span. *horizontal merge*
- `rowspan`: no of rows a cell should span. *vertical merge*