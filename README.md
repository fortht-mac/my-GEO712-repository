My GEO712 Repository
================
Tessa Forth
2026-10-05

------------------------------------------------------------------------

# Welcome to my GEO712 Repository!

I am creating this respository as part of Activity 2, after Session 3 on
using Git and GitHub.

*Notes for my future self on how I created this:*

- Generally, follow the **Activity** steps under [the Session
  page](https://github.com/paezha/Reproducible-Research-Workflow/tree/master/Session-04-Git-and-GitHub).

- I followed these steps using my Windows PC from Lab, rather than Linux
  Laptop.

  - This meant I had to re-install packages like `usethis` and
    `gitcreds`.

  - This also meant I had to create a new token for this new device.

    - I accidentally made a fine-grained token at first, which caused
      issues with Pull down the line - make sure to use Classic (even if
      you click the first option for Classic, there’s a second step you
      need to make sure you select correctly).

- I copied the contents of my original **Forth-Activity-1** R Markdown
  file, but importantly, it set the output as a `pdf_document`, so there
  was no corresponding .md. This gave issues when I tried to Commit.

  - To fix this, I set it to `output: github_document` (the same way the
    template README file auto-populates with), so that a .md file knits
    automatically.

------------------------------------------------------------------------

*Previous Activity’s contents below:*

------------------------------------------------------------------------

# Main Research Interests

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

# Favorites

## Favorite Music

1.  Spring Is Coming With A Strawberry In The Mouth: Roger Doyle & The
    Operating Theater
2.  Those Eyes, That Mouth: Cocteau Twins
3.  Hello Earth: Kate Bush
4.  The Predatory Wasp Of The Palisades Is Out To Get Us!: Sufjan
    Stevens
5.  Behind The Wheel: Depeche Mode

## Favorite Equation

*NDMI = (NIR-SWIR) / (NIR+SWIR)*

Where *NDMI* is the Normalized Difference Moisture Index, *NIR* is near
infrared reflectance, and *SWIR* is shortwave infrared reflectance.

## Favorite Artists

| Name | Achievements |
|----|----|
| John Nelson | A cartographer who makes beautiful maps and tutorials. My favorite is an animated map of the world’s oceans using the unique Spilhaus projection. |
| J.R.R. Tolkien | The author of the renowned fantasy trilogy “The Lord of The Rings,” as well as “The Hobbit” and “The Silmarillion.” |
| Michelangelo | Famous for painting the ceiling of the Sistine Chapel, as well as iconic sculptures such as the Pieta and David. |
| Francisco Goya | Known for expressive and thought-provoking paintings such as “The Third of May 1808” and “Saturn Devouring His Son.” |
| Pierre-Auguste Renoir | A French impressionist painter with works such as “Luncheon of the Boating Party” and “The Umbrellas.” |

# A Chunk of Code

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
