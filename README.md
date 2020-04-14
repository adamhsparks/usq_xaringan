# usq_xaringan

A xaringan theme that mimics the USQ corporate PowerPoint template.

![Slide showing code and graph slide layout](./man/code_graph_layout.png)

## Install

The template requires the [xaringan](https://github.com/yihui/xaringan) package by [Yihui Xie](https://yihui.name/), which provides an implementation of [remark.js](https://github.com/gnab/remark) through R Markdown.
It will be installed when you download usq_xaringan

```{r}
if (!require("remotes")) {
  install.packages("remotes", repos = "http://cran.rstudio.com/")
  library("remotes")
}

install_github("adamhsparks/usq_xaringan")
```

## Begin a slideshow

Use the usq_xaringan template in RStudio, go to `File` > `New File` > `RMarkdown...` > `From Template` > `Slide template for University of Southern Queensland`

You can also use the `draft()` function from the rmarkdown package:

```{r}
rmarkdown::draft(
  file = "your_presentation.Rmd",
  template = "usq_xaringan",
  package = "usq_xaringan"
)
```

