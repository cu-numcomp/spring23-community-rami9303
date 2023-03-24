# Community Software Analysis Proposal
Please edit this file and push to your repository.

## Software: Astropy

Astropy is an open source software Python package with the primary goal to provide a wide range of astronomy and astrophysics related functionality for professional and amateur astronomers and astrophysicists alike. Astropy is relevant to numerical computation in a number of ways. The Astropy package includes tools for interpolation and regression analysis of astronomical data. And uses numerical algorithms for data analysis, image processing, and modeling. Astropy also includes a subset of the SciPy library which is a collection of open source software for scientific computing. Specifically relevant to the course, it uses scipy.optimize which can be used for root finding. 

### Stats

| Description | Your answer |
|---------|-----------|
| Repository URL | https://github.com/astropy/astropy |
| Main/documentation website |https://www.astropy.org |
| Year project was started | 2011 |
| Number of contributors in the past year | 23 `git shortlog -se --since=2022-03-01` |
| Number of contributors in the lifetime of the project | 441 |
| Number of distinct affiliations | 6 institutions listed under Institutional Support. |
| Where do development discussions take place? | GitHub, Developer Email List, Slack, Open Astronomy Discourse forum, Google group |
| Typical number of emails/comments per week? | 2-3 emails on astropy-dev, 17 comments on Github issues |
| Typical number of commits per week? | Varies but average is 29 since week of Jan. 1, 2023 |
| Typical commit size | 0.54 KB/commit since Jan 01, 2023. git log --shortstat --since=2023-01-01 | awk '/^ [0-9]/ {commits++; insertions += $4; deletions += $6} END {size = (insertions + deletions) / 1024; print "avg commit size: " size/commits " kb/commit"}' |
| How does the project accept contributions? | Joining the astropy-dev mailing list/forum and pull requests |
| Does the project have an automated test suite? | Yes |
| Does the project use continuous integration? | Yes, CircleCI |
| Are any legal/licensing steps required to contribute? | No |

### Install and run

Check the following boxes when complete or add a note below if you
encountered a problem.

- [x] I have installed the software
- [x] I have run at least one example
- [x] I have run the test suite
- [x] The test suite passes

conda install -c conda-forge -c defaults scipy matplotlib \
  h5py beautifulsoup4 html5lib bleach pandas sortedcontainers \
  pytz setuptools mpmath bottleneck jplephem asdf pyarrow
Collecting package metadata (current_repodata.json): done
Solving environment: failed with initial frozen solve. Retrying with flexible solve.
Solving environment: failed with repodata from current_repodata.json, will retry with next repodata source.
Collecting package metadata (repodata.json): done
Solving environment: - 

| The test suite passes |
Test suite passes but 1 fails. test_core.py::test_rename_path

FAILED ../../../../../opt/anaconda3/lib/python3.9/site-packages/astropy/modeling/tests/test_core.py::test_rename_path
= 1 failed, 23081 passed, 236 skipped, 112 xfailed, 135 warnings in 227.40s (0:03:47) =
<ExitCode.TESTS_FAILED: 1>

### Notes/concerns/risks

"None at this time". I'm excited for this project because I have a passion for astronomy and believe this will be a great oppurtunity to learn more about the science behind it using the numerical computation concepts we have covered.  

#### Note on copyright
Students retain copyright on any work done in completion of a CU
course, so you are authorized to sign a [contributor license
agreement (CLA)](https://en.wikipedia.org/wiki/Contributor_License_Agreement),
affirm a [developer's certificate of
origin (DCO)](https://en.wikipedia.org/wiki/Developer_Certificate_of_Origin),
etc.  If you have concerns about this, please note them and/or reach
out to Jed directly.
