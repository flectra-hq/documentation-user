
.. |assistance-contact| replace::
   If you need Flectra assistance on this matter, please contact your Flectra Account Manager or contact
   our `Sales department`_.
.. _Sales department: mailto:sales@flectra.com

.. _db-upgrade:

=======
Upgrade
=======

.. _db-upgrade/overview:

Overview
========

.. _db-upgrade/process:

The upgrade process
-------------------

This documentation is for our *On-Premise* (self-hosted) and *Flectra.sh* customers. If you are hosted
Online, please check our :ref:`instruction page for our Online (SaaS) customers <upgrade_button>`.

.. _db-upgrade/definition:

Definition
~~~~~~~~~~

An upgrade is switching to a newer version of Flectra (e.g., Flectra 13.0 to Flectra2.0)

An upgrade does not cover:

* migration from another ERP to Flectra

.. note:: |assistance-contact|

.. _db-upgrade/process-workflow:

Process workflow
~~~~~~~~~~~~~~~~

The upgrade process in a nutshell:

#. You create a test upgrade request.
#. | The request is processed by Flectra:
   | This happens via an automated process that runs the database through an upgrade script and
     takes between 20 and 120 minutes. Only if an issue(s) arises will we have to intervene
     manually and adjust the script specifically to your database until the upgrade succeeds.
#. Flectra delivers a test database.
#. You test your database for possible discrepancies (see :ref:`db-upgrade/test-guidance`)
#. If there are any discrepancies, you report them to the Upgrade support team via the
   :ref:`Help portal <db-upgrade/test-assistance>`.
#. We will fix the issues and send you a new test database.
#. Once you completed the testing and are happy with the result, you decide on a date and time when
   you stop users from accessing Flectra, freeze all data entries and create an upgrade request for the
   production upgrade.
#. Flectra delivers the production database through the automated process.
#. You restore it in your Production environment a few short hours later and continue working on the
   newly upgraded database.

.. _db-upgrade/service-level:

Service Level Agreement
-----------------------

What is covered by the Enterprise Licence?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Databases hosted on Flectra’s Cloud platforms (Saas and Flectra.sh) or On-Premise (Self-Hosting) enjoy the
following service at all times.

The upgrade of:

* standard applications
* Studio customization (as long as the Studio app is still active)
* customizations done by our consulting and developer services *if* they are covered by a
  ‘Maintenance of Customisations’ subscription

The Upgrade Service is limited to the technical conversion and adaptation of your database (standard
modules and data) to make it compatible with the targeted version.

What upgrading does NOT cover
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* The cleaning of pre-existing data & configuration while upgrading
* Any new developments and/or upgrade of your own :ref:`custom modules
  <db-upgrade/faq/custom-modules>`
* `Training <https://www.flectra.com/learn>`_ on the new version




.. note:: |assistance-contact|

.. _db-upgrade/get-started:

Get started
===========

The upgrade process varies depending on where your database is hosted.

.. _db-upgrade/online:

Online (SaaS)
-------------

If you are hosted Online, please check our :ref:`instruction page for our Online (SaaS) customers
<upgrade_button>`.

On-Premise
----------

There are two possibilities:

#. Via the interface of our `website form <https://upgrade.flectra.com>`_
#. | For technically-advanced users and partners, via the following command line (to be used on the
     machine where your database is hosted):
   | ``python <(curl -s beta.upgrade.flectra.com/upgrade) test -d <your db name> -t2.0``

What does it do?
~~~~~~~~~~~~~~~~

The above command will dump your database to a file, then send it to the upgrade platform for
upgrade, displaying you the live logs, then restore the upgraded database back on your server as a
duplicate test database.

.. _db-upgrade/steps:

Steps
=====

.. _db-upgrade/steps-test:

The testing phase
-----------------

.. _db-upgrade/test-process:

Test process
~~~~~~~~~~~~

Also referred to as the pre-production phase, the test phase allows you to review an upgraded
version of your database without affecting your production database in any way.

We suggest that you run the test upgrade process at least once, but you can do it as often as you
want (one at a time).

Once you receive your upgraded test database, you should check that all data, processes and
functionality are still correct and working as expected.

If you do find discrepancies, you'll be able to:

* | :ref:`Report your issues <db-upgrade/test-assistance>`
  | and/or
* Ask for a new :ref:`test request <db-upgrade/test-db-request>` after the reported issues have
  been fixed in the upgrade script.

When you do not find any discrepancies, you'll be able to:

* Move on to the upgrade of your :ref:`production database <db-upgrade/production-live>`.

.. _db-upgrade/test-db-request:

Request a test database
~~~~~~~~~~~~~~~~~~~~~~~

When filling the `website form <https://upgrade.flectra.com>`_, select *Testing* purpose.

.. image:: media/db-upgrade-test-purpose.png
   :align: center
   :alt: Selection of the "Testing" purpose in the upgrade form on Flectra

.. _db-upgrade/test-guidance:

Test guidance
~~~~~~~~~~~~~

Every business and organization has its own operational needs and will have to test its specific
Flectra instance respectively. However, we recommend you look at `the test scenario
<https://drive.google.com/open?id=1Lm4JqbsHBirB1wMi14UChoz_YHLjx5ec>`_ we created, a high-level idea
of what you should test and look out for.

.. todo:: change link "test scenario" once the related doc is published

.. _db-upgrade/test-assistance:

Assistance
~~~~~~~~~~

If you encounter issues or problems in the **test database**, please contact the Flectra Upgrade
Support:

#. Connect to our `Flectra Support page <https://www.flectra.com/help>`_.
#. Under the *Ticket Description* section, select *An issue related to my upgrade* ticket type.

   .. image:: media/db-upgrade-test-assistance.png
      :align: center
      :alt: Selection of "An issue related to my upgrade" as Ticket Type in the support form on Flectra

   .. warning::
      If you choose another *Ticket Description* type, the request will be redirected to another
      team than the upgrade one and will slow down the processing and response time.

#. Please provide as much detail as you can. Where applicable, illustrate the current and previous
   flows with videos and/or screenshots. This will avoid clarifying questions and speed up the
   resolution process significantly.

   .. image:: media/db-upgrade-test-assistance-details.png
      :align: center
      :alt: "Detailed Description" field in the support form on Flectra

.. note::
   * The purpose of the test phase is not to correct existing data or configurations in your
     database.
   * |assistance-contact|

.. _db-upgrade/steps-production:

The production launch
---------------------

.. _db-upgrade/production-live:

Production goes live
~~~~~~~~~~~~~~~~~~~~

The production upgrade request is when you decide to upgrade your current database with all your
production data (invoices, VAT returns, inventories, current orders) to a new version of your choice.

After your :ref:`tests <db-upgrade/steps-test>` are completed to your satisfaction, submit the
request to upgrade your production database via our `website form <https://upgrade.flectra.com>`_.
Select *Production* purpose.

.. image:: media/db-upgrade-production-purpose.png
   :align: center
   :alt: Selection of the "Production" purpose in the upgrade form on Flectra

.. danger::
   Going into production without first testing may lead to:

   - business interruptions (e.g. no longer having the possibility to validate an action)
   - poor customer experiences (e.g. an eCommerce website that does not work correctly)

.. _db-upgrade/production-assistance:

Assistance
~~~~~~~~~~

If you encounter issues or problems in the **production database**, please contact the **Flectra
Support**:

#. Connect to our `Flectra Support page <https://www.flectra.com/help>`_.
#. Under the *Ticket Description* section, select the appropriate type related to your issue but
   **do not select** the option *An issue related to my upgrade*.

   .. note::
      After upgrading to production, the support will be provided by the Support team instead of the
      Upgrade team.

#. Please provide as much detail as you can. Where applicable, illustrate the current and previous
   flows with videos and/or screenshots. This will avoid clarifying questions and speed up the
   resolution process significantly.

   .. image:: media/db-upgrade-production-assistance-details.png
      :align: center
      :alt: "Detailed Description" field in the support form on Flectra

   .. warning::
      If you choose *An issue related to my upgrade* as ticket type, the request will be redirected
      to another team than the support one and will slow down the processing and response time.

.. _db-upgrade/faq:

FAQ
===

.. _db-upgrade/faq/why:

Why upgrade?
------------

* If you are in an :ref:`unsupported version <db-upgrade/supported-versions>`, you get a new version
  with support.

.. _db-upgrade/faq/when:

When to upgrade?
----------------

Whenever you want. You can make your upgrade request as soon as a new version is released on our
`website form <https://upgrade.flectra.com>`_.

.. _db-upgrade/faq/availability:

Availability of the new version
-------------------------------

Please kindly note that as soon as we announce the release of a new major version (usually at the
end of year), the Upgrade Service team needs to adapt the upgrade scripts to it, which is why the
new version is not immediately available for existing databases.

.. _db-upgrade/faq/finalization:

Finalization of the upgrade (:abbr:`ETA (Estimated Time of Arrival)`)
---------------------------------------------------------------------

Unfortunately, it is impossible to give time estimates for every upgrade request. Flectra offers so
many possibilities (e.g. branding, workflows, customization, etc) that it can get tricky to upgrade,
and translate to the new structure. If you use multiple apps managing sensitive data (e.g.,
Accounting, Inventory, etc.), some cases may still require a human intervention, making the process
slower.

This is especially true during the first months following the release of a new major version, which
can significantly lengthen the upgrade delay.

In general, the ‘smaller’ the database, the quickest the upgrade. A single-user database that uses
only CRM will be processed faster than a multi-company, multi-user database that uses Accounting,
Sales, Purchase, and Manufacturing.

So, in a nutshell, what can impact your upgrade lead time?

* Source & targeted versions
* Installed apps
* Volume of data
* Amount of customization (models, fields, methods, workflows, reports, website, etc.)
* Installation of new apps or configuration changes after the start of the test phase

Usually, the delays experienced during the first request (waiting time between the time you
submitted your first request for a test upgrade) can generally give you an idea of the time to wait
for the production request.

.. _db-upgrade/faq/custom-modules:

Upgrade of the custom modules
-----------------------------




If you have a custom code, you can choose to have it upgraded by our services, by one of our
`partners <https://www.flectra.com/partners>`_ or you can do it yourself.

.. note:: |assistance-contact|


Release Notes by version
------------------------

Open our `Release Note <https://www.flectra.com/page/release-notes>`_ page to get a summary of the new
features and improvements made in each version.

.. _db-upgrade/assistance:

Assistance
==========

.. _db-upgrade/contact:

Contact our Upgrade service support
-----------------------------------

Should you have any more questions about the upgrade, do not hesitate to send a message to `Flectra
Upgrade Team <mailto:upgrade@flectra.com>`_. We will be very pleased to answer it as soon as possible.

.. _db-upgrade/supported-versions:

Supported versions
------------------

Please note that Flectra provides support and bug fixing only for the three last major versions of Flectra.

This is a factor to take into consideration before upgrading. If you are on an older version, we
suggest you to prefer the most recent version to benefit from a longer support (before having to
upgrade again).

You can get more information about our :doc:`supported versions <../services/support/supported_versions>`.
