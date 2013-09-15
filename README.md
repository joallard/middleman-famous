Jon's Middleman Template
========================
This is Jon's Middleman template. It is Middleman bundled with
Foundation4, using HAML. It also uses some goodies like Livereload 
and a Google Analytics snippet.  There is no content by default. Because
it annoys me.

## (The same, in readable) Bullet points!
* Middleman
* Foundation 4
* HAML
* Livereload
* No content (annoying)
* Google Analytics

## Goodies
### Two-tier Layouts
In the layout folder, I put two layouts: `base`, and `layout`.
Basically, `layout` is `base` plus a frame to support stand-alone text.

That means you can drop in Markdown files which will layout correctly
in the grid without any more markup; while allowing you to customize
how your crafted HAML views look.

So for example, we can drop in `about.md` which will work as a
stand-alone document and use `layout`; as well as have `home.html.haml`
that will use `base` and configure rows in `home` rather than being in
the layout. 

For this to work, you only have to add `layout: base` in the
front-matter.

## Usage
### Install

    $ git clone git://github.com/joallard/middleman-jon ~/.middleman/jon

### Create

    $ middleman init [foo] --template=jon
    $ cd [foo]
    $ rm README.md    # because it's annoying

### Once in a while
    
    $ cd ~/.middleman/jon
    $ git pull [--rebase]   # if you want

## Improvements

* Make a branch for those who don't need the JS
* Make Analytics adaptable?

Corrections welcome. Enjoy!
