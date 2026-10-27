My GEO712 Repository
================
Tessa Forth,
Fall 2026

------------------------------------------------------------------------

# Welcome to my GEO712 Repository!

The goal of this repository is to practice using GitHub, as part of my
course: [Reproducible Research
Workflow](https://github.com/paezha/Reproducible-Research-Workflow/).

------------------------------------------------------------------------

# Repository Structure

- Folder: **Parent**
  - *Includes several setup files and the markdown files for the
    “homepage” *README*.*
  - Folder: **assets**
    - *Auxiliary images and data added as part of the assignment due
      10/28.*
    - *Initially populated with sample data/results figures from my
      research on tropical forest biomass growth trajectories, using an
      Ecoregion in Western Africa.*
  - Folder: **easter-egg**
    - *Created by Antonio as a contributor, including markdown and
      results for generating Tanaka contours of Mount Fuji.*
  - Folder: **notes**
    - *Notes I keep for myself each assignment/class, organized with the
      naming conventions: **AssignmentNotes_MM-DD** and
      **ClassNotes_MM-DD** respectively.*
    - Folder: **Rmd_Files**
      - *Keeping the more “back-end” files separate for simple
        navigation.*
  - Folder: **renv**
    - *Includes several setup files for a reproducible environment.*

------------------------------------------------------------------------

# About Me

## Academic History

- BA Environmental Studies: Lewis & Clark College (2026)
- MSc Earth & Environmental Sciences: McMaster University (In Progress)

## Main Research Interests

My principal areas of interest include:

- Tropical and coastal ecology

- Spatial analysis/remote sensing/GIS

- Carbon sequestration

At McMaster, I work with Dr. Alemu Gonsamo’s *Remote Sensing Lab.* My
research here centers on **how tropical forests recover their biomass
following stand-replacing disturbances.** My approach uses
*space-for-time substitution,* which means I quantify biomass from one
recent year, but across forests that were disturbed in different years.
That way, I can find a relationship between forest age and biomass,
essentially finding the rate of recovery over time.

Specifically, I am recording aboveground biomass estimations from
spaceborne LiDAR data, made available by the *GEDI L4A* product, and
relating this to forest loss data from the *Global Forest Change*
project.

------------------------------------------------------------------------

## Favorites

### Favorite Music

1.  Spring Is Coming With A Strawberry In The Mouth: Roger Doyle & The
    Operating Theater
2.  Those Eyes, That Mouth: Cocteau Twins
3.  Hello Earth: Kate Bush
4.  The Predatory Wasp Of The Palisades Is Out To Get Us!: Sufjan
    Stevens
5.  Behind The Wheel: Depeche Mode

### Favorite Equation

*NDMI = (NIR-SWIR) / (NIR+SWIR)*

Where *NDMI* is the Normalized Difference Moisture Index, *NIR* is near
infrared reflectance, and *SWIR* is shortwave infrared reflectance.

### Favorite Artists

| Name | Achievements |
|----|----|
| John Nelson | A cartographer who makes beautiful maps and tutorials. My favorite is an animated map of the world’s oceans using the unique Spilhaus projection. |
| J.R.R. Tolkien | The author of the renowned fantasy trilogy “The Lord of The Rings,” as well as “The Hobbit” and “The Silmarillion.” |
| Michelangelo | Famous for painting the ceiling of the Sistine Chapel, as well as iconic sculptures such as the Pieta and David. |
| Francisco Goya | Known for expressive and thought-provoking paintings such as “The Third of May 1808” and “Saturn Devouring His Son.” |
| Pierre-Auguste Renoir | A French impressionist painter with works such as “Luncheon of the Boating Party” and “The Umbrellas.” |

------------------------------------------------------------------------

# Sample Chunks of Code

## First Sample Chunk of Code

``` r
# Print the traditional first line of code, but adapted slightly to match a Kate Bush song title!
print("Hello Earth")
```

    ## [1] "Hello Earth"

``` r
# Calculate the first 5 powers of my favorite number
favoritenumber <- 4
powers <- favoritenumber^(1:5)
print(powers)
```

    ## [1]    4   16   64  256 1024

## Quote of the Day

``` r
# This quote changes every time you run/knit!
statquote()
```

    ## 
    ## Science is built up of facts, as a house is with stones. But a
    ## collection of facts is no more a science than a heap of stones is a
    ## house.
    ## --- Henri Poincare

------------------------------------------------------------------------
