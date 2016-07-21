presentations
================

# markdown and reveal.js

* many of these use pandoc to render from markdown to reveal.js
  * install pandoc `brew install pandoc`
  * if you did not clone with -r you need to init and update the revealjs submodule
    * `git submodule init; git submodule update`
  * if there is a Makefile, just type `make` to build the html
    * if not, look in the markdown file for building notes towards the top
      * if not, try something like `pandoc --slide-level 2 --css puppet.css -i --self-contained -t revealjs source.md -o output.html`
* pandoc is a bit opinionated in slide building and reveals when using {ahem} reveal.js
* in presentations that use reveal.js directly, just link to the relevent dirs in the reveal.js repo
  * (css, js, lib, plugin) and create a local index.html and it'll just-work
