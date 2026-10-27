Class Notes: October 21
================

Today’s session: [Projects and Reproducible
Environments](https://github.com/paezha/Reproducible-Research-Workflow/tree/master/Session-03-Projects-and-Reproducible-Environments)

------------------------------------------------------------------------

Synchronizing your local environment with the reproducible environment

*Type the following into the Console:*

- `renv::init()`
  - Scans the project to ensure it knows what’s needed, so that
    different devices contributing to the project can summon all the
    packages/environment specs.
  - Critical for ensuring the setup is reproducible and preservable
    across devices that may have different versions.
- `renv::status()`
  - Checks the current versioning status on your local device and how it
    aligns with the overall environment.
- `renv::restore()`
  - Can essentially re-align your own local library to the **renv.lock**
    file’s specification.
- `renv::snapshot()`
  - Update the **renv.lock** file according to your added libraries.
