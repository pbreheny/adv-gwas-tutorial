# Self-guided GWAS tutorial

Very much a work in progress. Uses the package [html](https://github.com/pbreheny/html) for rendering.

## Rendering

To turn all of the `.rmd` files into `.html` output,

``` r
html::render_all(list.files(".", "*.rmd"))'
```

The rendered files will appear in the `docs` folder.

Alternatively, you can render an individual page with

``` r
html::render_page('page.rmd')
```

This is often useful as it can take a long time to render the entire tutorial.

## Pushing

Changes to code can be pushed like usual, on the condition that the html files you want to push are in the `docs` folder.

## References to the packages we use

Here are the tools we use in the analysis steps presented here -- we recommend their documentation pages as references. All of these are open-source (freely available).

**Command-line tools**

-   [PLINK 1.9](https://www.cog-genomics.org/plink/1.9/)

-   [PLINK 2.0](https://www.cog-genomics.org/plink/2.0/)

**R packages**

-   [bigstatsr](https://privefl.github.io/bigstatsr/)

-   [bigsnpr](https://privefl.github.io/bigsnpr/)

-   [plmm](https://github.com/pbreheny/plmm)
