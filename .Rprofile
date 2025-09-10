source("renv/activate.R")

# Renv installation options: (1) use pak::pkg_install, which is faster, try to not install from source, download using curl, rely on Posit package manager, which can be more up-to-date.
options(
    renv.install.packages = pak::pkg_install,
    renv.install.from.source = "never",
    renv.download.method = "curl",
    repos = c(
        CRAN = "https://cloud.r-project.org",
        RSPM = "https://packagemanager.posit.co/cran/latest"))

library(tidyverse)
library(readxl)
library(ggpubr)         # Group multiple ggplots
library(ggrepel)        # Make circle plot text more legible
library(ggforce)        # For geom_circle()
library(feather)
library(igraph)
library(scales)         # For col_numeric() palettes
library(tidygraph)      # For static graphs
library(ggraph)
library(viridis)
library(ggthemes)       # Colorblind palette & tools to investigate palettes
library(ggtext)         # Apply styling to axis labels
library(glue)
library(gt)
library(janitor)        # adorn_totals() to add total row to tables
library(svglite)
# library(rbbt)           # Zotero citations

# Resolve conflicts
select <- dplyr::select
filter <- dplyr::filter
map <- purrr::map
