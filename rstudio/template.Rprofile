
library(packrat)
cat("You can manage your R packages through packrat.\n")
cat("More info under this link: ")
cat("https://rstudio.github.io/packrat/walkthrough.html\n\n")

library(rstudioapi)
.applyTheme <- function(){
  rsTheme <- Sys.getenv("R_ADD_RSTHEME")
  if (nchar(rsTheme) > 0) {
    rstudioapi::addTheme(rsTheme)
  }
  
  tmTheme <- Sys.getenv("R_ADD_TMTHEME")
  if (nchar(tmTheme) > 0) {
    rstudioapi::convertTheme(tmTheme)
  }
  
  theme <- Sys.getenv("R_APPLY_THEME")
  if (nchar(theme) > 0) {
    rstudioapi::applyTheme(theme)
  }
}
.applyTheme()
rm(.applyTheme)
cat("You can select your startup theme through R_APPLY_THEME environment variable.\n\n")
