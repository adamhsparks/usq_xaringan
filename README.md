# usq_xaringan

<!-- badges: start -->
[![Project Status: Unsupported – The project has reached a stable, usable state but I have ceased all work on it. If you wish to take over maintenance, please contact me.](https://www.repostatus.org/badges/latest/unsupported.svg)](https://www.repostatus.org/#unsupported)
<!-- badges: end -->

*usq_xaringan* is Unsupported

I have ceased all development and support for this R package.
If you work at USQ and wish to take over the maintenance and development of this package, feel free to contact me and let me know.
You can open an issue here to do this and ask me to transfer the repository to you.

A [***`xaringan`***](https://rmarkdown.rstudio.com/) theme that mimics the USQ corporate PowerPoint template.
The theme provides USQ typography and colours for your presentation in both slides and plots/graphs by default if using [***`ggplot2`***](https://ggplot2.tidyverse.org/) through the use of [***`theme.usq`***](https://adamhsparks.github.io/theme.usq/).

## Install

The template requires the [***`xaringan`***](https://github.com/yihui/xaringan) package by [Yihui Xie](https://yihui.name/), which provides an implementation of [remark.js](https://github.com/gnab/remark) through R Markdown.
It will be installed when you download ***`usq_xaringan`***.

```{r}
if (!require("remotes")) {
  install.packages("remotes", repos = "http://cran.rstudio.com/")
  library("remotes")
}

install_github("adamhsparks/usq_xaringan")
```

## Begin a slideshow

Use the ***`usq_xaringan`*** template in RStudio, go to `File` > `New File` > `R Markdown...` > `From Template` > `Slide template for University of Southern Queensland`

You can also use the `draft()` function from the [***`rmarkdown`***](https://rmarkdown.rstudio.com/) package:

```{r}
rmarkdown::draft(
  file = "your_presentation.Rmd",
  template = "usq_xaringan",
  package = "usq_xaringan"
)
```

## Example screenshots

### Title slide
![Title slide layout](./man/title_slide.png)


### Testimonial slide
![Testimonial slide layout](./man/testimonial.png)


### Code and graph layout
![Slide showing code and graph slide layout](./man/code_graph_layout.png)


### Final slide
![Final slide](./man/final_slide.png)

## Other features
[Fontawesome icons](https://fontawesome.com/) are supported through the [***`fontawesome`***](https://github.com/rstudio/fontawesome) library.
The icons on the final slide above are generated using this.

## Code of Conduct

Please note that the USQ.xaringan project is released with a [Contributor Code of Conduct](https://contributor-covenant.org/version/2/0/CODE_OF_CONDUCT.html). By contributing to this project, you agree to abide by its terms.
