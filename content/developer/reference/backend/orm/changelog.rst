.. _reference/orm/changelog:

=========
Changelog
=========

Flectra version 16.0
====================

- Translations for translated fields are stored as JSONB values with
  `#97692 <https://github.com/flectra/flectra/pull/97692>`_
  and `#101115 <https://github.com/flectra/flectra/pull/101115>`_.
  Code translations are no longer stored into the database.
  They become static and are extracted from the PO files when needed.

Flectra Online version 15.4
===========================

- New API for flushing to the database and invalidating the cache with
  `#87527 <https://github.com/flectra/flectra/pull/87527>`_.
  New methods have been added to `flectra.models.Model` and `flectra.api.Environment`,
  and are less confusing about what is actually done in each case.
  See the section :ref:`SQL Execution <reference/orm/sql>`.

Flectra Online version 15.2
===========================

- Specific index types on fields:  With `#83274 <https://github.com/flectra/flectra/pull/83274>`_ and
  `#83015 <https://github.com/flectra/flectra/pull/83015>`_, developers can now define what type of
  indexes can be used on fields by PostgreSQL. See the :ref:`index property <reference/fields>` of
  `flectra.fields.Field`.
