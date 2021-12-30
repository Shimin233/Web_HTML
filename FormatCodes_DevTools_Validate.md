## Format codes using Prettier
In the top menu, View - Command Palatte (Shift+Command+P) - Enter 'Format Documant' (Siift+Alt+F) - Configure - Enter 'Prettier-Code Formatter'

So that all codes are re-formatted by Prettier. To make codes formatted by Prettier every time, in the menu, Code - Setting (Command+,) - Search for 'Format on Save', enable this item, and the setting is completed; you can close the current tab of 'Setting' . 

## Inspect (and adjust) codes using Develop Tools in browser
Find 'Develop' from menu of Google Chrome (Command+Shift+I) or Web inspector for Safari (Command+Alt+I), look at Elements tab. 
- can see original codes for the current webpage, just like the html codes we typed
- can select part of codes that correspond to parts on webpage
  - enable or disable style items, or change value (like sizes; can type in numbers or use up/down arrows)
  - convenient to adjust look of webpage by looking at it simultaneously

## Validating web pages
#### Validating html
Go to the [webpage of this validator](https://validator.w3.org). 
As our webpage is now on the local computer, none else can enter it by URI; let us upload the index.html file instead. 
Then the validator can tell us what might be wrong with out webpage, like: 
- need `lang` for specifying the language used on the webpage
- need the attribute `alt` for the image `img`. 
- (temporarily ignore this)  The character encoding was not declared. Proceeding using windows-1252.
So we fix them: 
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
    </style>
  </head>
  <body>
    <img src="images/长歌2—大头.jpeg" alt="A profile image" />
    <p class="username">@whoever</p>
    <p>Hello world!</p>
  </body>
</html>
```
### Validating CSS
Go to this [CSS validator](https://jigsaw.w3.org/css-validator/). Now we can just validate by inputting (copying and pasting) all html codes(from index.html) into it, as we embedded all CSS in our html file. We will validate in another way as CSS becomes complicated. Here our current CSS is perfect, no error found. 

P.S. I tried uploading the index.html to validate CSS, it works in the same way as inputting - maybe this is not suitbale as CSS becomes complicated and no longer is embedded in html file. 
