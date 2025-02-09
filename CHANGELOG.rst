Changelog
~~~~~~~~~

Version 1.9.0
-------------

Backwards incompatible changes:

- limited supported versions of Python to 2.7, 3.5 and PyPy.
- limited supported Django versions to 1.7.10 and higher.
- turned off modeltranslation support by default (can be enabled)

Converted the test suite from doctest to unittest.

Bugs fixed:

- #25: max_length ignored in django 1.7 migrations
- #42: added setting to enable/disable modeltranslation support

Old versions
------------

Changelog before extracting to a separate repository::

  changeset:   23:34210c5b5b72
  user:        Andy Mikhailenko <neithere@gmail.com>
  date:        Sat Sep 27 05:55:42 2008 +0600
  summary:     Fixed bug in AutoSlugField: uniqueness check by date was broken

  changeset:   22:8b13c99f2164
  user:        Andy Mikhailenko <neithere@gmail.com>
  date:        Sat Sep 27 04:14:04 2008 +0600
  summary:     Rewrite AutoSlugField. Add optional attributes "unique" and "unique_for_date". Preserve "populate_from" as optional.

  changeset:   21:07aa85898221
  parent:      19:ae6294ba1162
  user:        Andy Mikhailenko <neithere@gmail.com>
  date:        Fri Sep 26 23:57:29 2008 +0600
  summary:     Use pytils for transliteration is AutoSlugField

  changeset:   12:e8b861b632d7
  user:        Andy Mikhailenko <neithere@gmail.com>
  date:        Wed Aug 06 07:26:39 2008 +0600
  summary:     Fix bug in custom_forms.auto_slug_field (missing import directive)

  changeset:   10:ac217f7edb53
  user:        Andy Mikhailenko <neithere@gmail.com>
  date:        Wed Aug 06 07:19:17 2008 +0600
  summary:     Add custom_models, including AutoSlugField
