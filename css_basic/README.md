Tasks
0. Some early styling
mandatory
Copy into this folder index.html and tweets.html that you created in the previous project:

Create an empty styles.css.
Create the file base.css and set the content of this file
In each of your HTML files, add these 2 lines within the <head> tag (do not confuse with the <header> tag!):

<link href="base.css" rel="stylesheet">
<link href="styles.css" rel="stylesheet">
If you refresh your webpages in your browser, they should now look a bit better!

We just told your webpages to use the CSS rules described in those two files, and to apply them to your HTML code.

Repo:

GitHub repository: alu-web-development
Directory: css_basic
File: base.css, styles.css, index.html, tweets.html
Please review your task manually with the following checklist
Files base.css, styles.css, index.html and tweets.html are present

0/2 pts
1. Positioning
mandatory
Even though each element of your webpages now has a different style, you may notice they still are stacked on top of each other, and that’s probably not what you want. CSS brings a few different approaches to positioning that one may use depending on cases.

For this project, we’re going to use CSS Flexbox, a recent set of CSS properties that work with recent browsers.

Our goal is to get a layout that looks like this:

Content of the <header> tag
Content of the <article> tag	Content of the <aside> tag
Content of the <footer> tag
As a reminder, there are also two container tags playing critical roles here:

<main> contains the area that includes <article> and <aside>.
<body> contains all of them together.
Here are steps to get this layout, which you will have to write as CSS code in the styles.css file:

Both container tags, <body> and <main> must be told that they are containers to flexible boxes: you need to apply the display: flex property to both of them.
However, <body> contains a column of three boxes (<header>, <main> and <footer>), therefore you must apply the flex-direction: column property to <body>; whereas <main> contains a row of 2 boxes (<article> and <aside>), so you must apply the flex-direction: row property to <main>.
Ensure the <main> tag keeps an automatic height and width, by applying the flex: auto property to it.
To wrap up the layout, you want to be sure that your content (article) takes ⅔ of the width of the page, and your aside takes ⅓; you can assign to them the number of boxes they should fill in. This is done by applying the property flex: 2 to <article> (using up 2 boxes), and flex: 1 to <aside> (using up 1 box).
Finally, you want to be sure that the user can scroll within your <article> and your <aside>. You can do this by applying the overflow-y: auto CSS property to both of them.
If you’ve done all of those properly, and your HTML structure is correct, you should get exactly the layout we were trying to get.

Do note that the exact rendering you’re getting may be slightly different depending on your browser (namely, about whether header and footer are fixed or not when the user scrolls), but should always match the layout presented above.

Repo:

GitHub repository: alu-web-development
Directory: css_basic
File: styles.css
Please review your task manually with the following checklist
File styles.css is present

0/6 pts
2. Responsive web design
mandatory
You may notice that the website keeps this layout when you make your browser window smaller, or visit it from a smartphone, and it’s unpleasant to use that way for your users. No worries, we covered this for you: just add the attribute class="works_on_smartphone" on the <body> tag in your index.html file, and the layout you just created will degrade nicely as you resize the window!

But you’ll notice, if you visit your website on a smartphone, that it will still have that layout, and just seem “zoomed out”. That’s because you need to adjust what is called the “viewport” of the browser when rendering the page. Hint: this gets done by adding a certain tag to your HTML code.

Repo:

GitHub repository: alu-web-development
Directory: css_basic
File: index.html, styles.css
Please review your task manually with the following checklist

