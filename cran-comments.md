## Test environments

* ubuntu 20.04 (local install), R 4.1.2
* macOS-latest (release, on GitHub Actions), R 4.1.2
* macOS-latest (devel, on GitHub Actions), R-dev
* ubuntu-latest (release, on GitHub Actions), R 4.1.2
* win-builder (release, devel)

## R CMD check results

0 errors | 0 warnings | 0 notes

-----

This version updates the writing locations to comply with CRAN policy by switching from using rappdirs::user_cache_dir("rnoaa/ersst") to using tools::R_user_dir("rnoaa/ersst", which = "cache").

The previous release had missed a use of rappdirs::user_cache_dir in the tests.

Thanks!
Daniel Hocking
