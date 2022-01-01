## Hyperlink
It is the `a` anchor element used for hyperlinks, to another html, or some non-html file like images, pdf, etc.
- Relative and absolute url address references
  - Relative url by `images/filename`, `company/filename`, where `images`, `company` are the folders under the current working repository(folder)
  - Relative url by `../filename`, where `..` double periods mean current working repository folder; can use in sequence `../../filename`, `../../../filename`
  - Absolute url by `/filename`, where `/`means the current working repository folder

- Let the link lead to downloading a file, by adding `download` right after the linked address i.e. the address of the file to be downloaded (delete `=''` as we do not need them here)

- Link to certain position on the same page
  - use `id` to define a position(or fragment, say) of a webpage and then use an `a` element with `#` to refer to it (just like \ref and \cite in LaTeX)

- Link to an exterior webpage like Google, in the same tab or a new tab (adding `target='_blank'` item right after the linked address
 The resulting codes are respectively, for index.html: 
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
    <a href="about.html">About Me</a>
    <a href="../HTML/"></a>
    <a href="company/about2.html">
      <img src="images/长歌2—大头.jpeg" alt="A clickable image" />
    </a>

    <a href="images/长歌2—大头.jpeg">My Photo (link to a non-html)</a>
    <a href="images/长歌2—大头.jpeg" download>Download My photo</a>
    <p class="username">@whoever</p>
    <p>
      Hello <em>world </em>and <i>everyone</i> <strong>here</strong> and
      <b>everywhere</b> !
    </p>
    <a href="#section-css">CSS</a>

    <a href="https://google.com">Google</a>
    <a href="https://google.com" target="_blank">Google in New Tab</a>
    <a href="mailto:sf686@cantab.ac.uk">Email Me</a>

    <h2>HTML</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde magnam
      minima nobis cumque? Quaerat accusantium magnam hic unde, itaque tenetur
      odio culpa cupiditate quod modi, necessitatibus aperiam! Obcaecati, error
      totam. Minima quos omnis at, quis asperiores ex architecto reprehenderit
      suscipit incidunt. Dignissimos numquam veritatis beatae optio magni
      aspernatur, cupiditate iure repudiandae aut? Itaque vitae id facilis
      eligendi aperiam eveniet libero laboriosam suscipit, maxime voluptate a at
      inventore vero animi atque corrupti autem quasi est quaerat reprehenderit?
      Saepe, perferendis sint? A non doloremque unde? Vel dolorem aspernatur
      ipsa aliquid culpa recusandae voluptatibus, esse iusto, nam autem
      perferendis ipsam iste, quod dicta quia debitis voluptates voluptas
      dolores velit! Voluptatum corporis rem consectetur, distinctio fuga
      nesciunt incidunt alias dolores repudiandae nobis dolorem rerum. Earum
      cumque aperiam repellendus vel nobis dignissimos reprehenderit ipsum a!
      Vel, molestias inventore. Sunt, rerum at voluptas ex quos repellendus ut
      molestiae non sit. Quam labore neque quos consectetur iure quibusdam quod,
      accusamus explicabo magnam voluptatum repellat pariatur deserunt, nisi cum
      sed ut impedit expedita autem iste nostrum asperiores facere maxime
      perspiciatis. Praesentium possimus velit quos aliquam magnam at ea
      voluptas consequuntur optio molestiae illo accusamus sint animi ex,
      repellat sit debitis. Quam, quibusdam debitis itaque facilis minus ut
      nemo?
    </p>
    <h2 id="section-css">CSS</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis odit,
      excepturi molestias suscipit asperiores dolorem quam maxime qui unde a
      expedita dignissimos ex quos sapiente officia voluptatibus atque voluptas.
      Quos corrupti ex excepturi qui vero officiis ipsum quidem atque eos dolor
      odio laboriosam, sapiente aspernatur, reprehenderit fuga placeat nemo,
      nulla necessitatibus! Doloribus laboriosam incidunt consectetur, ratione
      animi tenetur molestiae aliquam assumenda, voluptas a voluptatem
      accusantium dolorem? Officia, beatae expedita ab ducimus architecto rem
      saepe, quis nobis autem vitae soluta, nisi deleniti sapiente dolorem
      voluptatem. Aliquid quis deleniti hic expedita! Eaque vel cumque at,
      temporibus amet dicta dolore tempora aspernatur quas aut mollitia
      distinctio neque quibusdam nihil porro deleniti! Et minima harum ratione.
      Pariatur nesciunt magni, reprehenderit, quia vel accusantium ipsa velit
      aut tenetur quos quam quae, sed vero inventore optio minus repellat! In ad
      iure ullam accusantium alias aspernatur sed praesentium facilis sapiente
      cupiditate, quae laboriosam sequi aliquam natus quo tempore magnam nam
      ducimus asperiores amet blanditiis! Quis earum illum voluptates minus
      ducimus obcaecati vitae mollitia cupiditate alias facilis inventore porro
      quae modi, corporis laborum reiciendis. Earum architecto modi fugiat
      voluptatum atque cupiditate eaque dolorem, quaerat dolore quis aperiam
      accusamus! Commodi libero totam nesciunt! Similique optio nisi accusantium
      ipsum odit.
    </p>
    <a href="#">Jump to Top</a>
  </body>
</html>
```
... for about2.html: 
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <a href="../index.html">Home Page</a>
    <a href="../../">Relative url can be 1 to 3-layer; a bit hard to read</a>
    <a href="/index.html"
      >Absolute url, first slash means current folder; clearer for reading</a
    >
  </body>
</html>
```
## Images

## Tips
- Use command+F to search words in coding text 
- in `p` element, type `lorem200` would output a 200-in-length testing text
- Command+L+O (in this order!) to see resulting webpage in your browser
