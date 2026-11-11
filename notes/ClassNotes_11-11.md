Class Notes: November 11
================

Today’s session: [Documenting data analysis using R
Markdown](https://github.com/paezha/Reproducible-Research-Workflow/tree/master/Session-08-Documenting-Data-Analysis-with-RMarkdown)

------------------------------------------------------------------------

### Code chunk options in .Rmd files

- Code chunks, by default, print the output when you run them
  - This means echo = TRUE by default
  - Set echo = FALSE so that the code itself is suppressed
- You can also set eval = FALSE so that one block doesn’t always run
  when you run everything (eg initializing or installing packages, you
  don’t need to do that every single time you run the code).
- Can make it so that it detects if there has been a change in the code
  and re-runs, but only if there’s been a change.
- Can add labels for the chunk which helps navigation of the document,
  and lets you cross-reference (like “as I did in chunk 2…”)
- fig.cap is nice if the chunk will include a figure.

### Vignettes

- Appear as Articles in the actual package webpage
- Show up as a user’s guide/instructional materials as you’re sharing

#### Notes on creating a vignette

*I will need to re-do these steps on my Windows machine.*

- `usethis::us_vignette("myvignettetitle")`
  - Adds it in DESCRIPTION
  - Adds knitr, html, and r inside .gitignore inside the vignettes
    folder - these are just the byproducts.
  - Creates a template for you to modify, via .Rmd
    - Can modify the title, output, chunk options, and
- Write what is in your package, what you included and why, and why it’s
  important for someone else to know.

*Things I can include…*

- Title: “Report tropical forest biomass recovery trajectories at the
  ecoregion scale”

- Author: Tessa Forth

- Descriptive blurbs:

  - This package and repository were created as part of GEOG712:
    Reproducible Workflow in GitHub and R. The contents and function are
    adapted from my MSc thesis project, tentatively titled: “Evaluating
    the variability of tropical forest biomass recovery through a
    space-for-time synthesis of remote sensing datasets.”

  - This package uses a preliminary export file that has post-processed
    some ecoregion-level data on tropical forest biomass recovery rates,
    regression models, and nearby primary forest reference biomass. This
    data is derived primarily from the following sources:

    - RESOLVE Ecoregions: Dinerstein et al., 2017
      (<https://www.arcgis.com/home/item.html?id=37ea320eebb647c6838c23f72abae5ef#overview>)
    - GEDI L4A Aboveground Biomass Density, Version 2.1: Dubayah et al.,
      2020 (<a
      href="https://developers.google.com/earth-engine/datasets/catalog/LARSE_GEDI_GEDI04_A_002?_gl=1\emph%7B1sanpqq%7D_up\emph%7BMQ"
      class="uri">https://developers.google.com/earth-engine/datasets/catalog/LARSE_GEDI_GEDI04_A_002?_gl=1\emph{1sanpqq}_up\emph{MQ</a>..}\_ga\_ga_SM8HXJ53K2\*czE3ODk2NzEyMTEkbzEkZzAkdDE3ODk2NzEyMTEkajYwJGwwJGgw)
    - JRC Tropical Moist Forests Annual Change Collection: Vancutsem et
      al., 2021 (<https://forobs.jrc.ec.europa.eu/TMF/data>)

  - After exporting biomass and forest condition/age data sampled at
    GEDI footprint points in Google Earth Engine, resultant data were
    aggregated by ecoregion in Google Colab. This created
    *EcoregionExports.csv* which is a first-pass table of ecoregion
    results.

  - Subsequently, this package reads the export table, omits unnecessary
    data columns, and filters for records where ecoregion-level results
    were viable for reporting (i.e. no missing data, no negative growth
    slope, no excessively small R^2 values). It then calculates
    predicted biomass regrowth after 20 years, the percent of primary
    forest biomass that this constitutes, and the estimated time to
    reach the primary forest biomass benchmark. The final output is the
    *EcoregionResults* dataframe, which includes all these data ordered
    to highlight ecoregions with the fastest predicted recovery times.

- knitr include

- Setup –\> Load Libraries
