## Head section
In a black .html file (I created boilerplate.html for this), type `!` and click Tab, we will get a boilerplate html file, that is a basic template. 
Check out the items it uses:
- lang
- `charset` character set, it uses UTF-8, it is a character set like ASCII but it contains almost all characters in the world's languages
- `<meta name="viewport" content="width=device-width, initial-scale=1.0" />` it resizes the viewport part (the visible part) of the webpage (which can be resized by resizing the browser in practice) to fit with all computer monitors

can also add:
- keyword
- description

So the boilerplate looks like: 
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name='keywords' content='HTML, CSS'>
    <meta name='description' content='...'>
    <title>Document</title>
  </head>
  <body></body>
</html>
```

## Text

The `em` element, Emphasize, which is by default using _italic_ to stress the enclosed content
- can change the style of `em` in the `style` section

Can also change texts to _italic_ by `i` element
- but html is better to be used for structuring rather than styling, while CSS is for styling

The `strong` element is putting stress and importance to the enclosed text like `em`
- similarly, though it is by default __bold__ but this style can be changed

Can let text __bold__ using `b` element
- but again deprecated as `i` is, since we'd better use CSS for styling instead of html

A shortcut to produce `em` for text: 
- select the text we want to emphasise
- View-Command Palatte (command+shift+P) search for Wrap with abbreviation, and enter 'em', press return(enter), then the selected text is enclosed by `em` element as desired


```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>My First Web Page</title>
    <style>
      img {
        width: 120px;
        border-radius: 60px;
        float: left;
        margin-right: 10px;
      }

      p {
        font-size: medium;
      }

      .username {
        font-weight: bold;
      }
      em {
        color: red;
        font-style: normal;
      }
    </style>
  </head>
  <body>
    <img src="images/长歌2—大头.jpeg" alt="A profile image" />
    <p class="username">@whoever</p>
    <p>
      Hello <em>world </em>and <i>everyone</i> <strong>here</strong> and
      <b>everywherea</b> !
    </p>
  </body>
</html>
```
## Entities
