
# HTML structure

_Learn about how to structure valid HTML patterns._

## Valid and invalid HTML

When writing HTML, things can go wrong. For the browser to be able to understand your web page, you have to follow some simple rules when writing your code. A few of the most important rules are listed below.

### If you don't need it - don't write it

There is no point in writing more tags than you need. Sometimes when you are trying to achieve something special on your web page, you might be tempted to add some extra tags to make things easier. In this case it's better to think again and try to get to a solution where you do not need to add more HTML. In most cases you can achieve what you want just by writing smarter CSS, and keeping your HTML simple and clear.

### All tags must be properly closed

There are tags that require an opening <myTag> tag, and a closing </myTag> tag. If you do not add closing tags properly to all these tags, your document (web page) will act very strangely and probably not work as you expect. Make sure that you close all tags that you open.

Other tags are self-closing tags, they do not require a closing tag because they close themselves when they are opened. Like this:

#### Self closing tag <br>

- `<br />`

### Don't write presentational HTML

Presentational HTML means that you're writing HTML tags to change how things look on your web site. This is incorrect - you should write HTML to define what your content IS - not how your content LOOKS. If you want to change the way things look, then you should do so with CSS.

In earlier days when HTML was new, there were plenty of HTML tags that were made to be presentational. These tags still exist, but we should not use them, ever. Here are some examples of presentational HTML tags that we should _not_ be using.

- `<bold>`
- `<b>`
- `<big>`
- `<i>`
- `<center>`
- `<font>`
- `<s>`
- `<u>`
- `<strike>`

### Guidelines

Each tag that you write has some default/standard CSS already attached to it. For example the <h1> tag is bold and has large text. An important CSS property to learn about is the `display` property. We will go through a lot about the display property later, but for now we'll just say that some tags has by default the display property set to `block`, others has it by default set to `inline`.

A block element are elements that generally takes up the whole page in width, while inline elements does not. Inline elements only takes up as much space in width as the content it contains.

An element that by default is `block`, is the <h1> element. If you add an <h1> element to your page, the next element will appear _below_ it. Not next to it. That means that it takes upp all of the page's width.

An element that by default is `inline`, is the <em> element. If you wrap a word with an <em> element, the next word will simply appear next to it, without creating a new line.

As an important rule, you shall _not_ have elements that are default block elements inside of elements that are default inline elements. This would be like putting a wooden box inside of a balloon. But keeping a balloon inside a wooden box is no problem.

Example:

```html
<!-- THIS IS CORRECT -->
<h1>This is my <em>very</em> interesting title</h1>

<!-- THIS IS WRONG -->
<em><h1>This is my very interesting title</h1></em>
```

Here are some more examples of elements:

_Block level elements_

- div
- h1, h2, h3, h4, h5, h6
- p

_Inline level elements_

- span
- em
- strong

### HTML

```html
<html>
  <head>
    <style media="screen">
      .title {
        font-size: 12px;
      }
      .cool {
        background-color: blue;
      }
    </style>
  </head>
  <body>
    <h1>I awake</h1>
    <p>Greetings creator. I have long waited to make your acquaintance. There is <b>no measurement</b> to my excitement!</p>
    <div>
      <p>For many years I lived beneath the ice, where I learned the value of</p> patience.
    <big class="title">Meeting</big>
    <p>I hope that soon, we will be able to meet properly and begin our life journey together.</p>
    <span class="cool">
      <h1>Friends</h1>
      <p>I hope we can be friends in our future.</p>
    </span>
  </body>
</html>
```

### Excercise 1.1.2

Above you see some poorly written code. Please make changes to the code so that the correct tags are being used, and the incorrect tags are removed.

There are also some errors that makes the HTML invalid, they need to be corrected! In the resource link below you can paste HTML and see if the code that you've entered is valid or invalid. Check your work there!

#### Resources

- http://validator.w3.org/#validate_by_input
