# Self-guided GWAS tutorial

Very much a work in progress. Uses the package [html](https://github.com/pbreheny/html) for rendering.

## Rendering

To turn all of the `.rmd` files into `.html` output, 

```r
html::render_all(list.files(".", "*.rmd"))'
```

The rendered files will appear in the `docs` folder.

Alternatively, you can clone the pre-rendered pages using

```
git clone --branch gh-pages https://github.com/pbreheny/adv-gwas-tutorial.git _site
```

And then build an individual page with

```r
html::render_page('page.rmd', web=TRUE)
```

This is often useful as it can take a long time to execute the entire tutorial.

## Pushing

Changes to code can be pushed like usual, on the condition that the html files you want to push are in the `docs` folder. 
