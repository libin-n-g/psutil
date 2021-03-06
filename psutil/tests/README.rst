Instructions for running tests
==============================

* There are two ways of running tests. As a "user", if psutil is already
  installed and you just want to test it works::

    python -m psutil.tests --install-deps  # install test deps
    python -m psutil.tests

  As a "developer", if you have a copy of the source code and you whish to hack
  on psutil::

    make setup-dev-env  # install test deps (+ other things)
    make test

* To run tests on all supported Python versions install tox
  (``pip install tox``) then run ``tox`` from within psutil root directory.

* Every time a commit is pushed tests are automatically run on Travis
  (Linux, OSX) and appveyor (Windows):

  * Travis builds: https://travis-ci.org/giampaolo/psutil
  * AppVeyor builds: https://ci.appveyor.com/project/giampaolo/psutil
