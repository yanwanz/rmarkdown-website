
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rmarkdown-website

<!-- badges: start -->

<!-- badges: end -->

a template for creating a website in R Markdown

## Set up hosting

1.  Turn on hosting via GitHub Pages
    1.  Settings -\> GitHub Pages -\> select `docs/` folder
2.  View your website at given URL

## Maintainence

1.  Change content as necessary
2.  Render entire sites by running:

<!-- end list -->

``` r
rmarkdown::render_site("www")
```

1.  Commit and push changes.
    1.  Make sure to commit changes to **both** the `.Rmd` files in
        `www/` **and** the `.html` files in `docs/`
2.  Add new files as necessary
3.  Update `_site.yml` as necessary
