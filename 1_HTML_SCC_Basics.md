## HTML basics
Have Visual Studio Code downloaded (I chose the stable version). 

Create a folder (e.g. called 'HTML') on your computer (i did in my portable harddrive). 

Open VS Code, under 'Explorer' tab, click 'open folder' and choose your new folder 'HTML'. 

Click 'New File', and type its name as 'index.html', which is usually used as the home page of a website. 
In this file, type `<`, can see available codes - just click Return(Enter), get 
```html
<!DOCTYPE html>
```
where html code is not case-sensitive - but we often type everything in lowercase except `DOCTYPE` (though typing `doctype` is also fine).
- Start the html part, with the ending tab automatically appears. 
- Add head (with its ending tab automatically
  - Tip: just type `head` and click Tab, the first potential code will pop up
  -  In the head, add title
- Below head, add body
  - image  `img`, with source `src=''` (here we add a new folder alongside with index.html and drag a image into it beforehand) and (optional) alternate `alt=''` (to add more details to this image) (double or single quotation marks both work)
  - paragraph of texts, `p`
```html
<!DOCTYPE html>
<html>
    <head>
        <title>My First Web Page</title>
    </head>
    <body>
        <img src='images/img1.jpeg'>
        <p>@whoever</p>
        <p>Hello world!</p>
    </body>
</html>
```
See the result webpage by right-clicking the coding area - select Open with Live Server (command+L + command+C). 

## CSS basics
Further adjust formats of components on this webpage
In the head section: 
- add style
  - for the item `img`, adjust width, border-radius (taking it as half of the width will output a circle rather than a rectangle/square), float (locate it on the left) and margin-right(set a margin on its right)
  - for all the items `p`, font-size
  - if want to adjust some specific items among all the  `p`'s, can set class `username` and specify this class name by `.username{...}`, so that all the items with such a class name will have style applied to
```html
<!DOCTYPE html>
<html>
    <head>
        <title>My First Web Page</title>
        <style>
            img{
                width: 120px;
                border-radius: 60px;
                float: left;
                margin-right: 10px;
            }

            p{font-size: medium;}

            .username{
                font-weight: bold;
            }
        </style>
    </head>
    <body>
        <img src='images/长歌2—大头.jpeg'>
        <p class='username'>@whoever</p>
        <p>Hello world!</p>
    </body>
</html>
```



