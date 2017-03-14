<!-- README.md is generated from README.Rmd. Please edit that file -->
[![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/IQSSdevtools)](https://cran.r-project.org/package=IQSSdevtools)

IQSSdevtools
============

The goal of **IQSSdevtools** is to makes it easy to initialize and compile an R software package that complies with the IQSS Best Practices for Software Development and Sustainability (IBPSDS).

The package will contain three primary functions:

-   `init_iqss_package`: initialize a new IQSS Best Practices for Software Development and Sustainability compliant package

-   `add_iqss_package`: identify and add (when possible) missing Best Practice compliant elements from an existing R package

-   `build_iqss_package`: builds and tests IQSS Best Practice elements in an R package

IQSS Best Practices for Software Development and Sustainability \[R Language\]
==============================================================================

`init_iqss_package` initialises a skeleton package that allows you to begin to implement the IQSS Best Practices for Software Development and Sustainability.

-   **Documentation**: Sets up documentation dynamically generated using [RMarkdown](http://rmarkdown.rstudio.com/) and [roxygen2](https://CRAN.R-project.org/package=roxygen2). This includes a *README.Rmd* file along with a package websbsite generated with [pkgdown](https://github.com/hadley/pkgdown). The README.Rmd file should lay out core information about the package's motivation, methods and include a dynamically generated "quickstart" example. `init_iqss_package` also creates a *NEWS.md* file for you to document all changes made to the package by version.

-   **License**: Adds a [GPL-3 License](https://www.gnu.org/licenses/gpl-3.0.en.html)

-   **Version Control**: Sets up [git](https://git-scm.com/) version control.

-   **Source Code Hosting**: If a GitHub authentication token is provided with the `github_auth_token` argument, a new [GitHub](https://github.com/) remote repository is created for the package.

-   **Testing**: Sets up the infrastructure for [unit testing](https://en.wikipedia.org/wiki/Unit_testing) with the [testthat](https://CRAN.R-project.org/package=testthat) package. The basic foundation for external continuous integration of these unit tests is set up with the [Travis CI](https://travis-ci.org/) and [Appveyor](https://www.appveyor.com/) services to run the tests on Linux and Windows operating systems, respectively.

Relationship with `devtools`
============================

**IQSSdevtools** largely builds on the [devtools](https://CRAN.R-project.org/package=devtools) package. It wraps many of the **devtools** functions based on the Best Practices. As such, feel free to use any **devtools** function when developing your package to add additional elements/run specific functions.
