PACKAGE-BUILDER RELEASE HISTORY
===============================
Go [here](https://github.com/PSLmodels~/Package-Builder/pulls?q=is%3Apr+is%3Aclosed)
for a complete commit history.


2019-04-15 Release 0.22.0
-------------------------
(last merged pull request is
[#164](https://github.com/PSLmodels/Package-Builder/pull/164))

**API Changes**
- None

**New Features**
- Simplify `--local` so that it is a simple boolean option and allow the locally installed package to be specified with any version
  [[#164](https://github.com/PSLmodels/Package-Builder/pull/164)
  by Martin Holmer]

**Bug Fixes**
- None

2019-03-13 Release 0.21.0
-------------------------
(last merged pull request is
[#161](https://github.com/PSLmodels/Package-Builder/pull/161))

**API Changes**
- None

**New Features**
- None

**Bug Fixes**
- Correct name of directory where built package is to be found for local installation using the new `--local LOCAL` option
  [[#161](https://github.com/PSLmodels/Package-Builder/pull/161)
  by Martin Holmer]


2019-03-13 Release 0.20.0
-------------------------
(last merged pull request is
[#158](https://github.com/PSLmodels/Package-Builder/pull/158))

**API Changes**
- Remove `--also37` option as now packages for uploading are automatically built for both Python 3.6 and Python 3.7
  [[#158](https://github.com/PSLmodels/Package-Builder/pull/158)
  by Martin Holmer]

**New Features**
- Add `--local LOCAL` option to build package from local source code and install it on local computer
  [[#158](https://github.com/PSLmodels/Package-Builder/pull/158)
  by Martin Holmer with suggestion and assistance from Hank Doupe]

**Bug Fixes**
- None


2018-12-19 Release 0.19.0
-------------------------
(last merged pull request is
[#153](https://github.com/PSLmodels/Package-Builder/pull/153))

**API Changes**
- None

**New Features**
- Add datetime to :starting and :finishing prints
  [[#153](https://github.com/PSLmodels/Package-Builder/pull/153)
  by Martin Holmer]

**Bug Fixes**
- None


2018-12-18 Release 0.18.0
-------------------------
(last merged pull request is
[#150](https://github.com/PSLmodels/Package-Builder/pull/150))

**API Changes**
- None

**New Features**
- Use newer `subprocess.run` in `os_call` utility function
  [[#150](https://github.com/PSLmodels/Package-Builder/pull/150)
  by Martin Holmer]

**Bug Fixes**
- None


2018-12-17 Release 0.17.0
-------------------------
(last merged pull request is
[#149](https://github.com/PSLmodels/Package-Builder/pull/149))

**API Changes**
- None

**New Features**
- Add `anaconda upload` command print statement
  [[#149](https://github.com/PSLmodels/Package-Builder/pull/149)
  by Martin Holmer based on suggestion from Hank Doupe]

**Bug Fixes**
- None


2018-12-16 Release 0.16.0
-------------------------
(last merged pull request is
[#148](https://github.com/PSLmodels/Package-Builder/pull/148))

**API Changes**
- None

**New Features**
- Make `anaconda upload` command overwrite already uploaded packages
  [[#148](https://github.com/PSLmodels/Package-Builder/pull/148)
  by Martin Holmer with assistance from Hank Doupe]
- Avoid using the new 1.7.* versions of anaconda-client package
  [[#148](https://github.com/PSLmodels/Package-Builder/pull/148)
  by Martin Holmer with assistance from Hank Doupe]

**Bug Fixes**
- None


2018-12-15 Release 0.15.0
-------------------------
(last merged pull request is
[#147](https://github.com/PSLmodels/Package-Builder/pull/147))

**API Changes**
- None

**New Features**
- Simplify `anaconda upload` command used by Package-Builder
  [[#147](https://github.com/PSLmodels/Package-Builder/pull/147)
  by Martin Holmer with assistance from Hank Doupe]

**Bug Fixes**
- None


2018-12-15 Release 0.14.0
-------------------------
(last merged pull request is
[#146](https://github.com/PSLmodels/Package-Builder/pull/146))

**API Changes**
- None

**New Features**
- Add `anaconda-client` as a required dependency of Package-Builder
  [[#146](https://github.com/PSLmodels/Package-Builder/pull/146)
  by Martin Holmer with need pointed out by Hank Doupe]

**Bug Fixes**
- None


2018-12-14 Release 0.13.0
-------------------------
(last merged pull request is
[#144](https://github.com/PSLmodels/Package-Builder/pull/144))

**API Changes**
- Add `pbrelease` options `--also37` and `--dryrun` so that packages for Python 3.7 can also be built and uploaded, and so that the build/upload plan can be viewed without executing the plan
  [[#136](https://github.com/PSLmodels/Package-Builder/pull/136)
  by Martin Holmer]

**New Features**
- None

**Bug Fixes**
- None


2018-11-14 Release 0.12.1
-------------------------
(last merged pull request is
[#126](https://github.com/PSLmodels/Package-Builder/pull/126))

**API Changes**
- None

**New Features**
- Add easier-to-understand error message to `pbrelease` CLI if Anaconda token file is not present
  [[#125](https://github.com/PSLmodels/Package-Builder/pull/125)
  by Martin Holmer]
- Make `git clone` faster by downloading only repository code for the version being released (rather than the whole repository)
  [[#126](https://github.com/PSLmodels/Package-Builder/pull/126)
  by Martin Holmer]

**Bug Fixes**
- None


2018-11-13 Release 0.12.0
-------------------------
(last merged pull request is
[#123](https://github.com/PSLmodels/Package-Builder/pull/123))

**API Changes**
- Change `pbrelease` CLI error handling to show simpler error messages and help
  [[#123](https://github.com/PSLmodels/Package-Builder/pull/123)
  by Martin Holmer]

**New Features**
- None

**Bug Fixes**
- None


2018-11-13 Release 0.11.0
-------------------------
(last merged pull request is
[#120](https://github.com/PSLmodels/Package-Builder/pull/120))

**API Changes**
- Change approach to specifying the package version
  [[#120](https://github.com/PSLmodels/Package-Builder/pull/120)
  by Martin Holmer]

**New Features**
- None

**Bug Fixes**
- None


2018-11-12 Release 0.10.0
-------------------------
(last merged pull request is
[#118](https://github.com/PSLmodels/Package-Builder/pull/118))

**API Changes**
- Add `pbrelease`, a command-line interface (CLI) to Package-Builder
  [[#118](https://github.com/PSLmodels/Package-Builder/pull/118)
  by Martin Holmer]

**New Features**
- Don't stop on `anaconda upload` errors because they may be caused by existence of packages already on Anaconda Cloud channel
  [[#116](https://github.com/PSLmodels/Package-Builder/pull/116)
  by Martin Holmer with assistance from Joseph Crail]
- Add `conda build purge` command as part of clean-up activities as recommended by output generated by one of the Anaconda utilities
  [[#116](https://github.com/PSLmodels/Package-Builder/pull/116)
  by Martin Holmer]

**Bug Fixes**
- None


2018-11-11 Release 0.9.0
------------------------
(last merged pull request is
[#112](https://github.com/PSLmodels/Package-Builder/pull/112))

**API Changes**
- Massive redesign of Package-Builder logic along the lines of Hank Doupe's
  `builder.py` script (originally checked in on 2018-05-31) with elements of
  Joseph Crail's prior approach (developed during 2017)
  [[#112](https://github.com/PSLmodels/Package-Builder/pull/112)
  by Martin Holmer with major assistance from Hank Doupe and Joseph Crail]

**New Features**
- None

**Bug Fixes**
- None


Before Release 0.9.0
--------------------
See commit history for pull requests before
[#103](https://github.com/PSLmodels/Package-Builder/pull/103)
