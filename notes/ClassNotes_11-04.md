Class Notes: November 4
================

Today’s session: [Creating packages in R and documenting
datasets](https://github.com/paezha/Reproducible-Research-Workflow/tree/master/Session-07-Creating-R-Packages-and-Documenting-Data)

------------------------------------------------------------------------

### Typed in Console:

- `install.packages("remotes")`
- `remotes::install_github("paezha/packr",                         build_vignettes = TRUE)`
- `library(packr)`
- `?packr`
  - Shows a fun new doc in the Help pane
- `data(package = "packr")`
  - Shows available datasets in a new popup (energy & emissions)
- `?energy_and_emissions`
  - No results found for now, not in the documentation

Purpose of **.gitignore:** Can create “secrets” files and share them
offline, that way it’s backed up but not public.

### Create a package

- Good to work in a new project, since nesting projects is a bad idea.
- For naming, `install.packages("available")` and `library(available)`
  - Then `available("testpackagenamehere")`
  - Name can’t have spaces, can’t start with a number
- `usethis::create_package("/home/tessa/Code/R/Course_RepWorkflow/tropicalforestbiomass")`
- `usethis::use_tidy_description()`
  - Then edit the info for setup & clarity
- `usethis::use_mit_license()`
- `devtools::document()`
- `install.packages("devtools", dependencies = TRUE)`
- `> usethis::use_readme_rmd()`
- `usethis::use_git()`

Aha! I had a hiccup. My Linux likes me to re-establish the token every
time, and turns out, my token had expired. So I followed this process:

- Created a new classic token in Github on browser.
- `gitcreds::gitcreds_set()`
  - Pasted in the new token
- `usethis::use_github()`
- Then, it was able to connect and establish a [new
  repo](https://github.com/fortht-mac/tropicalforestbiomass) to my
  GitHub account

Later:

- `usethis::use_r("name")`
  - Creates a new R script in a folder called **R**
- Go to **Build** and click **Install**
  - Create a new R script

Still couldn’t get devtools…

- Typed this into Terminal:
  - `sudo apt-get update`
  - `sudo apt-get install libxml2-dev pkg-config`
  - `sudo apt-get install libfontconfig1-dev`
- Actually so that didn’t work.
