=========
Changelog
=========

0.4.0 (2023-06-11)
------------------

.. note::

    The 0.4.0 release mainly has had a project management overhaul. The project has
    transferred to the Jazzband organization. This release mostly focuses on Python/Django
    version compatibility and organization of tests, CI etc.

    Many thanks for people who reported bugs, and especially, your patience for getting
    this release on PyPI.


**Breaking changes**

* Dropped support for Django 2.2, 3.0, 3.1 and 4.0
* Dropped support for Python 3.6 and 3.7

These versions are (nearly) end-of-life and no longer supported by their upstream teams.

**New features**

* Implemented settings for cookie flags: SameSite, HttpOnly, Secure, domain (#27, #60,
  #36, #88)
* Added Dutch translations

**Bugfixes**

* Cache instance resolution is now lazy (#41)
* Fixed support for Django 4.1 (#73) - thanks @alahdal
* Fixed default settings being bytestrings (#24, #55, #69)
* Fixed the middleware to clean cookies (#13) - thanks @some1ataplace
* Fixed bug in JS ``beforeDeclined`` attribute

**Project maintenance**

* Transferred project to Jazzband (#38, #64, #75)
* Replaced Travis CI with Github Actions (#64, #75)
* Set up correct test matrix for python/django versions (#75)
* Code is now ``isort`` and ``black`` formatted (#75)
* Set up ``tox`` and ``pytest`` for testing (#64, #75)
* 'Removed' the example app - the ``testapp`` in the repository is still a good example
* Configured tbump for the release flow
* Confirmed support for Python 3.11 and Django 4.2
* Added explicit template tag tests (#39)

**Documentation**

Did some initial restructuring to make the docs easier to digest, more to come.

* Added documentation on how to contribute
* Corrected settings documentation (#53, #14)
* Documented ``cookiebar.js`` usage (#90) - thanks @MrCordeiro
* Added better contributor documentation and example app documentation based on the
  ``testapp`` in the repository.

0.3.1 (2022-02-17)
------------------

- Protect against open redirect after accepting cookies (#48)


0.3.0 (2021-12-08)
------------------

* support ranges from django 2.2 to 4.0 and python 3.6 to 3.9


0.2.6 (2020-06-17)
------------------

* fix: setup for python 2.7


0.2.5 (2020-06-17)
------------------

* chore: add package descriptions


0.2.4 (2020-06-17)
------------------

* Cookie Bar Choosing Decline Not Disappearing Right Away (#22)

* 📦 NEW: pt_BR (#23)

0.2.3 (2020-06-15)
------------------

* Update package classifiers


0.2.2 (2020-06-15)
------------------

* 8732949 Remove jquery (#20)


0.2.1 (2020-06-02)
------------------

* fix: Set max version for django-appconf (#18)

* fix: Views ignore 'next' url parameter (#12)

* Update configuration.rst


0.2.0 (2020-02-11)
------------------

* support ranges from django 1.9 to 3.0 and python 2.7 to 3.7 (JonHerr)

0.1.1
-----

* tweak admin

* Add accepted_cookies template filter

* Add varname property to Cookie model

* Add translation catalog

0.1.0
-----

* Initial release
