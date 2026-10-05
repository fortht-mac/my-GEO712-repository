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
