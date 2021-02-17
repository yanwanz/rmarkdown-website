
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rmarkdown-website

<!-- badges: start -->
<!-- badges: end -->

a template for creating a website in R Markdown

## Set up hosting (once)

1.  Fork this repository.
2.  Turn on hosting via GitHub Pages
    1.  Settings -&gt; GitHub Pages -&gt; Source -&gt; select “master
        branch `/docs` folder”
3.  View your website at given URL
    1.  <https://YOUR-GITHUB-USERNAME.github.io/rmarkdown-website/>

## Maintainence

1.  Change content as necessary
    1.  Modify existing `.Rmd` files
    2.  Add new files as necessary
    3.  Update `_site.yml` as necessary
2.  Render entire site by running:

``` r
rmarkdown::render_site("www")
```

1.  Commit and push changes.
    1.  Make sure to commit changes to **both** the `.Rmd` files in
        `www/` **and** the `.html` files in `docs/`

## Adding a new blog post

1.  Create a new `.Rmd` file.
2.  Write the new blog post in the new `.Rmd` file.
3.  Render the website.
4.  Commit and push.

### Security

Please note that [all pages hosted via GitHub Pages are public on the
internet](https://docs.github.com/en/github/working-with-github-pages/about-github-pages),
even if the repository is **private**!!

However, there are few steps you can take to reduce the chance of your
blog post going viral. Please note that these are [security by
obscurity](https://en.wikipedia.org/wiki/Security_through_obscurity)
techniques that are NOT robust.

1.  Put it on the [deep web](https://en.wikipedia.org/wiki/Deep_web).
    Most search engines *crawl* the web. If there are no links to a URL,
    then crawlers will never find it. Just don’t link to your blog post
    **anywhere**. \[Note: it’s possible that the GitHub Pages service
    might index all pages. \]
2.  You can at least make the URL harder to remember or copy-and-paste
    by pading the name with a random MD5 hash.

``` r
obscure_filename <- paste0(
  "post_",
  digest::digest(runif(1), algo = "md5"),
  ".Rmd"
)
obscure_filename
#> [1] "post_60cd546dc6eac59c385073535502e5b2.Rmd"
```

## Consider adding your resume

You might consider writing your resume in **pagedown** and adding it to
your website. Like these:

-   <https://pagedown.rbind.io/html-resume>
-   <http://nickstrayer.me/cv/>
-   [Documentation](https://pagedown.rbind.io/#fig:resume-relaxed)

## Resources

-   [R Markdown
    websites](https://bookdown.org/yihui/rmarkdown/rmarkdown-site.html)
-   [Bootstrap 3.3
    components](https://getbootstrap.com/docs/3.3/components/)
-   [Bootswatch themes](https://bootswatch.com/3/)
-   [Font Awesome icons](https://fontawesome.com/icons?d=gallery&m=free)
-   [**bsplus**](https://ijlyttle.github.io/bsplus/articles/bsplus.html)
    package for additional Bootstrap components
-   📣: [**bslib**](https://rstudio.github.io/bslib/) library for
    Bootstrap theming
