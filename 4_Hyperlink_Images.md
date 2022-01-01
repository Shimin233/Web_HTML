## Hyperlink
It is the `a` anchor element used for hyperlinks, to another html, or some non-html file like images, pdf, etc.
- Relative and absolute url address references
  - Relative url by `images/filename`, `company/filename`, where `images`, `company` are the folders under the current working repository(folder)
  - Relative url by `../filename`, where `..` double periods mean current working repository folder; can use in sequence `../../filename`, `../../../filename`
  - Absolute url by `/filename`, where `/`means the current working repository folder

- Let the link lead to downloading a file, by adding `download` right after the linked address i.e. the address of the file to be downloaded (delete `=''` as we do not need them here)

- Link to certain position on the same page
  - use `id` to define a position(or fragment, say) of a webpage and then use an `a` element with `#` to refer to it (just like \ref and \cite in LaTeX)

- Link to an exterior webpage like Google, in the same tab or a new tab

## Images
