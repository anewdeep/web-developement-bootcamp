# Getting started with CSS

## Welcome to CSS
- **CSS** used to style elements in web page.
- Styling language that works with HTML to giva a page its look and layout.

    <img src = "https://lecontent.sololearn.com/material-images/0f80a6870bb34bd3b2801691249f288f-1.01.01_.gif" height = "300" style = "display:block; margin-left:auto; margin-right:auto">

- CSS builds on top of HTML. `style` attribute allows creating CSS properties to customize visual representation of HTML elements.
- *color* property controls the color of the text.
- color, border, font-size, margin are examples of CSS properties.
- CSS properties require values. Values are possible settings for a property.
- CSS properties and values are separated with a colon.
- CSS code for an HTML element must be enclosed in quotes.
- To apply multiple CSS properties, separate them with semi-colon.

    <h2 style = "color:red; background-color:black; text-align:center">Game Over</h2>

- CSS stands for **Cascading Style Sheets** and it is one of the 3 core web technologies.

## Styling techniques
- The styling technique that adds CSS code inside HTML elements is called **inline CSS**.

    <img src = "https://lecontent.sololearn.com/material-images/83fa4775e5ea4a4592d72f6f550dd7a1-explore.png" style = "display:block; margin-left:auto; margin-right:auto;" height = 140>

- Easy to add to HTML elements but applying the same style to more than one element, CSS code needs to be repeated.
- **Internal CSS** used to style the entire page.
- `<style>` container tag added to HTML document to group all CSS code for the page.

    <img src = "https://lecontent.sololearn.com/material-images/0058d8dc8002461ca59a543656654485-M1L2LP7.png" style = "display:block; margin-left:auto; margin-right:auto;" height = 180>

- **Selector** in CSS code matches the HTML tag to be targeted.

    <img src = "https://lecontent.sololearn.com/material-images/dfd9005eb09846feaa4ab3ac30e8613d-M1L2LP13.png" style = "display:block; margin-left:auto; margin-right:auto;" height = 100>

- Separate multiple selectors with comma to apply the same style to different elements.

    ```
        <style>
            h3, p {
                color: orchid;
                text-align: center;
            }
        </style>
    ```

## The anatomy of CSS
- CSS code creates styling rules.
- Simplest styling rule consists of a selector, plus declaration in curly braces.

    <img src = "https://lecontent.sololearn.com/material-images/783c011e3e144afda19a7efed8009312-M1L3LP4.png" style = "display:block; margin-left:auto; margin-right:auto;" height = 100>

- Can add as many declarations to the rule as needed, each one ending with a semi-colon.
- Declaration consists of a property and a value. They always come in pairs, separated by a colon.

    <img src = "https://lecontent.sololearn.com/material-images/87accf3bb7d44d1c8c66b76c41e31d65-M1L3LP8.png" style = "display:block; margin-left:auto; margin-right:auto;" height = 100>

- CSS code can contain as many styling rules as needed.

## Style Inheritence
- HTML nesting: some tags that go inside others.
- Outer element is parent, inner element is child.
- Styling rules for parent, will also be applied to the child elements by default (**CSS inheritence**).
- For child to different styles, write separate rules for the child.
- **Descendant selector**: targets only the elements that are nested within other elements.
`parent_selector child_selector{property:value;}`
    ```
        <!-- styles only the bold text nested within h1>
        h1 b{
            color: blue;
        }
    ```

## ID and class selectors
- `id` attribute identifies unique elements in an HTML document.
- Specific elements can be targeted using hash followed by `id` as a selector.
    ```
        <style>
            #heading {
                background-color: blue;
                color: yellow;
                text-align: center;
            }
            #movie {
                background-color: yellow;
                color: blue;
                text-align: center;
            }
        </style>
        <h2 id = "heading">Movie</h2>
        <h2 id = "movie">Palm Springs</h2>
    ```
    <img src = "https://i.ibb.co/jh0B0QV/image.png" style = "display: block; margin-left: auto; margin-right: auto;">

- `class` attribute is used to give the same identifier to a group of elements.
- Group of elements in the same class can be targeted using dot followed by the class name.
    ```
        .movie {
            color: white;
            background-color: black;
        }
    ```
- To only target specific elements of a certain class: `element_name.class_name {styling rules}`
    `p.content` targets all paragraph elements with class name "content".
- An elemenet can have both, a class, and an id.
- Each type of CSS selector has a priority.
    <img src = "https://lecontent.sololearn.com/material-images/d8b62b76ca1e488d9566ba23f7774b7e-M1L6Lp6.png" width = 300
    style = "display: block; margin-left: auto; margin-right: auto">
- This priority order is known as **specificity** which is an algorithm used by browsers to determine the rule to apply to an element.
- Comments in CSS code snippet enclosed in `/* ... */`.
- External css code written outside the HTML doc in a separate file. Same CSS style can be used by multiple HTML doc/web pages.
- Styling can be done without adding style tags in external CSS.

# Styling elements

## Introduction to color
- `color`, `background-color`
- **Color model**: way of representing and recreating real colors using codes. **RGB** is one of the most used models.
- RGB model creates colors by combining different intensities of red, green, and blue. (range 0-255)
- rgb(255, 255, 255) represents white.
    ```
        p {
            color: rgb(127, 255, 212);
        }
    ```
- Colors in rgb model can also be represented as **HEX codes**.
    <img src = "https://lecontent.sololearn.com/material-images/68f712def7f448729697a8a8bf6735b7-M2L7LP12.png" height = 100
    style = "display: block; margin-left: auto; margin-right: auto">
- HEX codes start with hash symbol, followed by 3 pairs of characters, each representing the intensity of r, b & b accordingly.
- Each character in a HEX code can have one of the 16 possible values (0-9 and A-F). 00 being the least intense, and FF being the most intense.

## Dimensions
- Screen display made up of picture elements or **pixels**.
- Pixels used as measuring unit to control dimentions of an element.
- `font-size` property controls text size.
    ```
        button {
            font-size: 15px
        }
    ```
- Most web browsers have default text size for paragraphs, buttons, lists as **16px**.
- Values such as small, medium, and large can be used. They already have set pixel values.
    - small: 13
    - medium: 16
    - large: 18
- Modern websites are built to look great on screens of different sizes and resolutions. This approach is called **responsive web design**.
- Using pixels as a measurement unit is not the best practice when it comes to resposive web design as screens come in different sizes and resolutions.
- Percentages are used to set relative dimensions.
    ```
        img {
            width: 50%;
        }
    ```
- WHen styling elements use percentages, 100% would be the full size of its parent element.
- If the width of an HTML element is set to 50%, it'll take half of its parent's width.
- Percentages can be used to set font sizes. Font sizes will be calculated using parent's font size as reference.

## Styling text
- `text-align`: aligns text. left, right, center, justify
- `text-decoration`: underline, overline, line-through, underline overline
- Some CSS properties can take multiple values.
- Color for decoration can be changed by adding color name, rgb, or hex code after decoration type.

    ```
        <body>
            <p class = "underline">underline text</p>
            <p class = "overline">overline text</p>
            <p class = "line-through">line-through text</p>
            <p class = "underline_overline">underline overline text</p>
        </body>

        body {
            font-size: 3em;
            text-align: center;
            background-color: black;
            color: white;
        }

        .underline {
            text-decoration: underline dotted red
        }

        .overline {
            text-decoration: overline dashed green
        }

        .line-through {
            text-decoration: line-through double blue
        }

        .underline_overline {
            text-decoration-line: underline overline;
            text-decoration-style: wavy;
            text-decoration-color: yellow
        }
    ```

    <img src = "https://i.ibb.co/7z5BRQw/image.png" width = 400
    style = "display: block; margin-left: auto; margin-right: auto">
- `text-transform`: controls capitalization of text content.

    ```
        <body>
            <p class = "capitalize">this is capitalized.</p>
            <p class = "lowercase">THIS IS LOWERcase</p>
            <p class = "uppercase">This is uppercase</p>
        </body>

        body {
            font-size: 3em;
            text-align: center;
            background-color: black;
            color: white;
        }

        .capitalize {
            text-transform: capitalize;
        }

        .lowercase {
            text-transform: lowercase;
        }

        .uppercase {
            text-transform: uppercase;
        }
    ```

    <img src = "https://i.ibb.co/f9B94LC/image.png" width = 400
    style = "display: block; margin-left: auto; margin-right: auto">
- `text-shadow`: creates a depth effect, gives emphasis, or add a stylish touch to the typography. Requires two values- horizontal offset and vertical offset. Accepts 2 additional and optional values- blur radius and color.

    ```
        <body>
            <h1 id = "movie">LAW & ORDER</h1>
        </body>

        body {
            font-size: 2em;
            text-align: center;
            background-color: black;
            color: white;
        }

        #movie {
            text-shadow: 1px 1px 2px red, 0 0 1em blue, 0 0 0.2em blue;
        }
    ```

    <img src = "https://i.ibb.co/0scNhnC/image.png" width = 500
    style = "display: block; margin-left: auto; margin-right: auto">

## Font styles
- Fonts play a crucial role in web design, influencing readabililty, aesthetics and UX.
- `font-family`: specifies typeface of the text
- Many fonts are installed by default in all devices. These are **web safe fonts**.
- Other fonts need to be installed on the user's device.
- Web safe fonts are specifed as a backup in case the user doesn't have a font installed.
- Arial, Courier New, Times New Roman, Trebuchet MS, Verdana, Tahoma
- `font-family` specifies a list of fonts from highest to lowest priority. Font selection stops at the first font in the list that is on the user's system.
- **Generic font families** are groups of fonts with similar typefaces. Used as universal fallbacks. Best practice to place them as the last option in a font-family property. If the preferred fonts are unavailable, browsers will use a font from that family.

    <img src = "https://lecontent.sololearn.com/material-images/760a347d4c814400bc4a3e7edaec86bc-23.png" width = 500
    style = "display: block; margin-left: auto; margin-right: auto;">
- `font-weight` controls the thickness or boldness of the text.

    <img src = "https://lecontent.sololearn.com/material-images/d7e77fae46884fd2a050eca27c208352-M2L10LP14.png" width = 500
    style = "display: block; margin-left: auto; margin-right: auto">

    ```
        <body>
            <h1 id = "serif">LAW & ORDER</h1>
            <h1 id = "sans-serif">her</h1>
            <h1 id = "monospace">[the social network]</h1>
            <h1 id = "cursive">Diary of a Wimpy Kid</h1>
            <h1 id = "fantasy">Harry Potter</h1>
        </body>

        body {
            font-size: 1.5em;
            text-align: center;
            background-color: black;
            color: white;
        }

        #serif {
            text-shadow: 1px 1px 2px red, 0 0 1em blue, 0 0 0.2em blue;
            font-family: serif;
        }
            
        #sans-serif {
            text-shadow: 1px 1px 2px red, 0 0 1em blue, 0 0 0.2em blue;
            font-family: sans-serif;
            font-weight: 800;
        }

        #monospace {
            text-shadow: 1px 1px 2px red, 0 0 1em blue, 0 0 0.2em blue;
            font-family: monospace;
        }

        #cursive {
            text-shadow: 1px 1px 2px red, 0 0 1em blue, 0 0 0.2em blue;
            font-family: cursive;
        }

        #fantasy {
            text-shadow: 1px 1px 2px red, 0 0 1em blue, 0 0 0.2em blue;
            font-family: fantasy;
        }

    ```

    <img src = "https://i.ibb.co/QCz6mGQ/image.png" width = 400
    style = "display: block; margin-left: auto; margin-right: auto">

## Styling links
- A link, by default is underlined and blue in color which can be overriden with CSS.
- The look of links that haven't been visited yet, can be changed using CSS.
- When user interacts with a link or any other element, it changes its state.
- Different states of an element can be targeted by using **pseudo selectors**.

    ```
        <body>
            <a class = "youtube" href = "youtube.com">YouTube</a><br>
            <a class = "twitch" href = "twitch.com">Twitch</a>
        </body>

        body {
            background-color: black;
            color: white;
        }

        a { 
            display: block;
            color: white;
            line-height: auto;
            text-decoration: None;
            font-family: Arial;
            font-size: 2em;
            font-weight: 900;
            text-align: center;
            transition: color 0.3s, font-size 0.3s;
        }

        a.youtube:hover {
            color: red;
            font-size: 3em;
        }

        a.twitch:hover {
            color: purple;
            font-size: 3em;
        }

        a:active {
            font-size: 2em;
        }
    ```

    <img src = "https://i.ibb.co/HpN7hfW/image.png" style = "display: block; margin: auto">
- By default links are underlined. Set `text-decoration: None` to remove underline.

## Styling tables
- Look of an HTML table can be greatly with the `border` property.
- Border refers to 3 sub properties: `border-width`, `border-style`, and `border-color`.
- The only required sub-property is style.
- If width not mentioned, default is *1px*.
- If color not specified, text color becomes border color.
- Table cells have spacing between them by default, making double borders appear. To remove spaces, give table element `border-collapse: collapse;` property.
- Table can have multiple rows as children. Pseudo selectors can be used to target elements based on their order or position.
    `tr:nth-child(5) {}` targets 5th row in the table.
- nth-child selector can also be used to target odd and even rows. `nth-child(odd) | nth-child(even)`

    ```
        <body>
            <!-- Table with a broder around the table -->
            <table id="table1">
                <tr>
                    <th>Rank</th>
                    <th>Movie Title</th>
                    <th>Director</th>
                </tr>
                <tr>
                    <td>1</td>
                    <td>Mulholland Drive</td>
                    <td>David Lynch</td> 
                </tr>
                <tr>
                    <td>2</td>
                    <td>The portrait of a lady on fire</td>
                    <td>Celine Sciamma</td>
                </tr>
                <tr>
                    <td>3</td>
                    <td>La Haine</td>
                    <td>Mathieu Kassovitz</td>
                </tr>
            </table>
            <!-- Table with a broder on all cells -->
            <table id="table2">
                <tr>
                    <th>Rank</th>
                    <th>Movie Title</th>
                    <th>Director</th>
                </tr>
                <tr>
                    <td>1</td>
                    <td>Mulholland Drive</td>
                    <td>David Lynch</td> 
                </tr>
                <tr>
                    <td>2</td>
                    <td>The portrait of a lady on fire</td>
                    <td>Celine Sciamma</td>
                </tr>
                <tr>
                    <td>3</td>
                    <td>La Haine</td>
                    <td>Mathieu Kassovitz</td>
                </tr>
            </table>
        </body>

        body {
            font-family: Arial, sans-serif;
            background-color: #F7F8FC;
        }

        /* Applying the border around the table */
        #table1 {
            border: 2px solid #0C1527;
        }

        /* Applying borders to each cell */
        #table2 {
            border-collapse: collapse;
        }

        #table2 th,
        #table2 td {
            border: 2px solid #0C1527;
        }

        td {
            text-align: left;
        }

        th {
            text-align: left;
            background-color: #149EF2
        }

        #table2 tr:nth-child(odd) {
            color: black;
            background-color: powderblue;
        }

        #table2 tr:nth-child(even) {
            color: powderblue;
            background-color: black;
        }
    ```

    <img src = "https://i.ibb.co/NtYp0M9/image.png" style = "display: block; margin: auto">

## Styling lists
- By default, unordered list items are marked with round bullets (disc).
- `list-style` property takes 3 values: type, position, image.
    ```
        ul {
            list-style: square inside none
        }
    ```
- Unordered list style types: square, circle, disc, none.
    <img src = "https://lecontent.sololearn.com/material-images/b883e3fd72cf4f1b93289f82ba718cf7-M2L13LP5.png" width = 450450
    style = "display: block; margin: auto">
- Ordered list style types: decimal, decimal-leading-zero, lower-roman, upper-roman, lower-alpha, upper-alpha
    <img src = "https://lecontent.sololearn.com/material-images/942efc24bd904851a22aa3a6820cbfab-M2L13LP10.png" width = 450450
    style = "display: block; margin: auto">
- `list-style-position`: inside, outside
    <img src = "https://lecontent.sololearn.com/material-images/87b4f8b435e34379a610f7bc4c1c4c9d-Frame37481.png" width = 450450
    style = "display: block; margin: auto">
- `list-style-image`: add custom image as a marker
    `list-style-image: url('../rocket.png')`

## Styling forms
- Inputs and labels can be styled with element selectors.
- By default, input elements have borders.
    ```
        /* To remove borders from input element*/
        input {
            border: none;
        }
    ```
- Input elements come in different types.
- Different types can be targeted using `[attribute]` selector.
    ```
        input[type = "text"], input[type = "email"] {
            property: value;
        }
    ```
- `border-radius` rounds corners of elements giving them a softer appearance.
- When border-radius is given a single value, it applies uniform rounding.
- border-radius takes percentages as well, which are calculated relative to the dimensions of the element.
- 50% radius to a square shaped element, turns it into a circle.
- To apply different values to different corners, provide a list of 4 values, separated by spaces in order from top-left to bottom-left clockwise.
- Just for links, pseudo selectors style different states of a button.

    ```
        <form>
            <label for="name">Name: </label>
            <input type="text" id="name">
            <br><br>
            <label for="email">Email: </label>
            <input type="email" id="email">
            <br><br>
            <input type="submit" value="Send">
        </form>

        body {
            background-color: #0c1527;
        }

        input[type="text"],
        input[type="email"] {
            border: 1px solid #ff9e03;
            background-color: #17233b;
            color: #ffffff;
            font-weight: bold;
            border-radius: 10px;
        }

        input[type="submit"] {
            background-color: #149ef2;
            border-radius: 10px;
            border: none;
            font-weight: bold;
            color: white;
        }

        input[type="submit"]:hover {
            background-color: #0c1527;
            color: #ff9e03;
            border: 1px solid #ff9e03;
            border-radius: 10px;
        }

        label {
            font-weight: bold;
            color: #ff9e03;
        }
    ```

    <img src = "https://i.ibb.co/D16Gv7Z/image.png" style = "display: block; margin: auto" width = 450>

# Page Design & Layout

## The box model
- **Box model** treats HTML elements as a rectangular box with 4 layers.
    <img src = "https://lecontent.sololearn.com/material-images/6250104032a244a8baf815bf7caa2133-52.png" width = 450
    style = "display: block; margin: auto; padding: 15px">
- **Content box** is the innermost layer where content like text and images appear.
- `width` and `height` properties set the side of the content box for an element.
- HTML elements can be classified into **inline** and **block** elements.
- By default, when width and height is not set, block elements take up the full width available (given by its parent).
- By default, inline element have a content layer that takes up as much width as necessary to display the content.
- `text-align` property aligns text within the content box of an element.
- By default, **border** is applied on the edges of box content, unless **padding** has been added.
- **Padding layer** is wrapped around content box to create extra space within the element and push border outwards.
- Padding is the distance between content and its border.
- **Border** is the third layer that surrounds the padding.
- Different padding values can be given for each of the 4 sides in order: top right bottom left (`padding-top` `padding-right` `padding-bottom` `padding-left`)
- To calculate total box dimensions, add together the dimensions of the 3 layers: content, padding and border.
- **Margin** is the outermost layer in box model. Wraps around the border layer and is transparent.
- Like padding, margin can be set individually for all 4 sides.

    ```
        <html>

        <head>
            <title>Block-level elements</title>
        </head>

        <body>
            <h2>Block-level element 1</h2>
            <div>
                <p>Block-level element 2</p>
            </div>
            <a href="#">Inline element</a><br><br>
            <div class="default-box">
                Element without padding and margin
            </div> <br>
            <div class="custom-box1">
                Element with padding
            </div> <br>
            <div class="custom-box2">
                Element with padding and margin
            </div>
            </div>
        </body>

        </html>

        body {
            background-color: #0c1527;
            color: white;
        }

        .default-box {
            border: 2px solid #ffa310;
        }

        .custom-box1 {
            padding: 10px;
            border: 2px solid #ffa310
        }

        .custom-box2 {
            padding: 10px;
            border: 2px solid #ffa310;
            margin: 10px;
        }

        div {
            width: 50%;
        }
    ```
    <img src = "https://i.ibb.co/Njk7cqm/image.png" width = 600400
    style = "display: block; margin: auto; padding: 15px">

## Flexbox layout
- `display` property overrides default behaviour of inline and block elements.
- Images are inline elements by defuault. To turn them into a block element
    ```
        img {
            display: block;
        }
    ```
- Similarly, paragraph, a block element, can be converted to inline.
    ```
        p {
            display: inline;
        }
    ```
- **Flexbox** layout makes it easier to build and design responsive pages. It creates a row or a column layout.
- Flexbox arranges items inside a container automatically.
- By default, child items inside a flex parent container are arranged automatically in a single row.
- `flex-direction`: row/column
- `flex-wrap`: wrap/nowrap - Items arranged automatically abd bynver if lines depends on screen size.
- `flex-grow`: 1, 2, 3, ... - Gives items ability to grow to take up more space.
- `flex-shrink`: 1, 2, 3, ... - Determines how much a flex item will shrink.

## Positioning
- By default, all elements are positioned **static**. Browser will display them one after another, in the order they appear in the HTML code.
- Elements can be given an exact position using pixels as coordinates.
- `position` property gives more control on where to place the HTML elements.
- `position: absolute` gives elements exact position.
- Add horizontal and vertical coordinates using `left` and `top`.
- Positioning an HTML element, means positioning one of its corners.
- Applying `position: absolute` to an element takes it out of its static flow (element order).
- Element with `position: fixed` always stays in the same place even when the page is scrolled.
- Use `position: relative` to reposition an element without taking it out of the static flow.
- **Relative** makes the element's static position, the new reference.
- To precisely position child elements in relation to position of the parent, set parent to `position: relative`.
- Relative and absolute are used in combination to position child elements in relation to their parents.
- If parent has no set position, the reference will be the nearest ancestor with property set to relative.
- In addition to `left` and `top`, `right` and `bottom` can also be used to position elements.

## Backgrounds
- `background-color` set colour of the background.
- `background-image: url("image.png")` set an image file as the background.
    <img src = "https://lecontent.sololearn.com/material-images/fa989fb43ab9487dab759915c77fc2a5-56.png" width = 400
    style = "display: block; margin: auto; padding: 15px">
- If the image is smaller than the canvas, image gets repeated by default to cover all the painting area.
- `background-repeat: no-repeat` image appears only once in the top left corner.
- `background-repeat: repeat-x(repeat-y)` control tiling direction.
    <img src = "https://lecontent.sololearn.com/material-images/431674c1d46d4bf1bc9ae2e07fdc9c45-57.png" width = 400
    style = "display: block; margin: auto; padding: 15px">
    1. no-repeat
    2. repeat-x
    3. repeat
    4. repeat-y
- `background-position: 10px 7px` places the background image 10px from the left and 7px from the top.
- `background-position` can take pixels, percentages and words (top, bottom, left, right and center).
    <img src = "https://lecontent.sololearn.com/material-images/20dfbcc212e4478cbebdf27b75b87a41-59.png" width = 400
    style = "display: block; margin: auto; padding: 15px">
- `background-size` controls the dimensions of the background image (width height).
    <img src = "https://lecontent.sololearn.com/material-images/acc23135f8d6410e99c31357b3ace74b-60.png" width = 400
    style = "display: block; margin: auto; padding: 15px">
- **contain** scales the image to ensure the entire image is shown as big as possible. Can result in tiling or empty spaces.
- **cover** scales the image completely over the canvas.

# Transitions and Transforms

## Transforms
- Transformtaions are usually triggered by user actions.
- `transform: translate` repositions an element horizontally and/or vertically. Providing 1 single value moves it horizontally.
    <img src = "https://lecontent.sololearn.com/material-images/e220829089d94362ae68c6c44be0a303-M4L19LP2.png" width = 400
    style = "display: block; margin: auto; padding: 15px">
- Transformations are not permanent changes. They are used to create visual effects.
- When **translate** used with 2 values, the visual effect moves the element both horizontally and vertically.
- Positive values translate an element to the right and down. Negative, left and up.
    <img src = "https://lecontent.sololearn.com/material-images/118a8f3b0daa41ecafc0bd6b4c065299-M4L19LP4.png" width = 400
    style = "display: block; margin: auto; padding: 15px">
- `transform: scale` makes an element bigger or smaller, preserving its aspect ratio. The original size has a value of 1, so a value of 2 will double the width and height. 0.5 will halve them.
- `transform: rotate` to rotate elements. (45deg- 45 degrees clockwise, -15deg- 15 degrees anti-clockwise).
- By default, rotations take place around the center of the element. `transform-origin` to change the point around which the rotation takes place. Requires the horizontal and vertical position of the new point of reference. 
    <img src = "https://lecontent.sololearn.com/material-images/cab5b024057f40688c219b1067f5e464-M4L19LP15.png" width = 400
    style = "display: block; margin: auto; padding: 15px">
- A combination of transformations can be applied to an element.
    ```
        div:active {
            transform: translate(100px, 150px)
            rotate(70deg) scale(1.5);
        }
    ```

## Transitions
- An **animation** produces visual effects of change in HTML elements.
- **CSS transitions** are changes in an element poroperties that happen over a period of time.
    <img src = "https://lecontent.sololearn.com/material-images/3c92d6ffd3854c87a46ce0b22cb8d1ff-72.png" width = 400
    style = "display: block; margin: auto; padding: 15px">
- A transition requires at least: a **property** (that will change), its **inital value**, its **final value**, a **duration**, and a **trigger**.
    <img src = "https://lecontent.sololearn.com/material-images/39c386bae43d439ea3c40ddf30ad2c2d-73.png" width = 400
    style = "display: block; margin: auto; padding: 15px">
- Multiple properties can be changed in a single transition. Each set of instructions to change a property are separated by commas.
    `transtition: background-color 0.5s, font-size 1s, width 0.5s`.
- `transition-delay` adds a waiting time before the transition effect.
- Transition effects can be added to transformations.
    ```
        <button>Press and hold</button>

        button {
            padding: 10px 20px;
            font-size: 16px;
            margin: 30px;
            border: none;
            border: radius 5px;
            background-color: blue;
            color: white;
            transition: transform 1s;
        }

        button:active {
            transform: scale(2)
        }
    ```

## Keyframes and animations
- Animations are used to produce more complex animations with more intermediate states. Change as many properties as needed, and as many times as needed.
- Animations need **keyframes** to hold the styles that the element will have at certain times.
- An animation is a sequence of transitions.
- **Keyframes** are snapshots with important intermediate states that define an animation.
    <img src = "https://lecontent.sololearn.com/material-images/2aaa6b5a8b60411cac223bbee2f03bfc-74.png" width = 42.5%><img src = "https://lecontent.sololearn.com/material-images/87729dc29cf642dbbf89f2b023064e4c-75.png" width = 50%>
- New animation needs to be given an `animation-name`. Use `@keyframes` followed by the `animation-name` to define the intermediate states.
- `animation-duration` controls the time it takes for the element to move from the first keyframe to the final one.
- `animation-delay` adds a waiting time for the animation to start playing.
- Can use `from` and `to` instead of using percentages, if there are only two key frames.

## Animation properties
- Transitions between 2 keyframs are smooth and calculated automatically based on the **speed function**. Speed function controls how fast the changes happen at different phases of the animation. 
- Frames between 2 keyframes are automatically generated basd on the speed function.
- Default speed function is **ease** which speeds up first, then slows down.
- `animation-timing-function` to set alternatives to the default speed.
    <img src = "https://lecontent.sololearn.com/material-images/7ce05e59aa5e4cd4b29795d66478157d-82.png" width = 400
    style = "display: block; margin: auto; padding: 15px">
    1. ease: speeds up first, then slows down.
    2. linear: constant speed.
    3. ease-in: starts slow, then speeds up.
    4. ease-out: starts fast, then slows down.
- `animation-iteration-count` determines the number of times an animation repeats.
- To make an animation repeat forever, use **infinite** value with `animation-iteration-count`.
- `animation` property can be used as a shorthand for all animation related properties.
    <img src = "https://lecontent.sololearn.com/material-images/d37747a39845480a9412d524ad41f438-M4L22LP16.png" width = 400
    style = "display: block; margin: auto; padding: 15px">