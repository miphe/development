
# HTML Semantics

_Learn the fundamentals about HTML and how to correctly write meaningful markup._

HTML - Hyper Text Markup Language - is a simple tag language that lets you declare what content your web page has. It's a way to 'tag', or 'mark' up your content so that a browser, bots and non-human things can understand what it is.

HTML is also a way to structure your web site so that there's a way for us as humans to know what your web page is or can do.

Without HTML, a web page would just be text with no way to know what that text means in relation to itself - for instance, we wouldn't know what text is the title, or what part of the text is a navigation or what part of the page that is the main part compared to an advertisement.

## Semantics

This is a word that has huge _meaning_ in HTML - semantics. It basically means "meaning" or "meaningfulness". If you _semantically_ write your web page with the correct tags, a robot should be able to make sense out of it. The robot should be able to tell what is a title, what is a link or a menu. That is why using the correct tags is very important.

As an example, consider the following code.

### HTML

```html
<html>
  <head>...</head>
  <body>
    <div class="title">Hello my friend</div>
    <div> class="text">It has been a long time since I wrote, I have been finding it difficult to make time.</div>
    <div class="text">
      My faculty here at <span class="acronym">SUOAE</span> are keen on keeping us busy at all times. <br /> I am learning a lot about biology and chemistry, this is <span class="emphasize">imperative</span> in my research on the creation of life.
    </div>
  </body>
</html>
```

### CSS

```css
.title {
  font-size: 2rem;
}
.text {
  font-size: 1.2rem;
}
.acronym {
  color: #999;
  font-weight: bold;
}
.emphasize {
  text-style: italic;
}
```

In the above example, we are only using non-semantic HTML tags (div, span). They are considered non-semantic because they don't really have much meaning. A `div` and a `span` doesn't mean much to a robot when it's trying to read your web page, therefore it will not know if your title is a title, or if your acronym is an acronym, to the robot it is just text and every word is just as important as the other. This is a problem.

### Excercise 1.1.1

Create an HTML file and a CSS file with the example above, but where you have used the _correct semantic tags_ instead of the non-semantic tags `div` and `span`. By thinking about what 'role' the text has in it's context, you can figure out which HTML tag would be appropriate.

#### Resources

- https://www.w3schools.com/tags/default.asp
