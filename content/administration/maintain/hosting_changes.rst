
.. _db_management/hosting_changes:

=======================
Change hosting solution
=======================

You may want to move your Flectra database from one hosting solution to another.
Depending on the platforms, you have to do it by yourself or contact our support team first.

From on-premises to Flectra Online
==================================

1. Create a :ref:`duplicate <duplicate_premise>` of your database: in this duplicate, uninstall all the **non-standard apps**.
2. Grab a "dump with filestore" of your database by using the Database Manager.
3. **If you have time constraints, contact us earlier to schedule the transfer.**
4. `Create a support ticket <https://www.flectra.com/help>`_ and attach the dump (if the file is too large, use any file transfer service and attach the link to your ticket). Also include your subscription number and the URL you want to use for your database (e.g.: my-company.flectra.com).
5. We will make sure your database is compatible and upload it to our cloud. In case of technical issues, we will get in touch with you.
6. It's done!

.. important::
   - Flectra Online is not compatible with **non-standard apps**.
   - The database you are moving to Flectra Online must be in a :doc:`supported version
     <supported_versions>`.

From on-premises to Flectra.sh
==============================

1. Follow the :ref:`Import your database section of the Flectra.sh documentation <odoo_sh_import_your_database>`.
2. ...and voilà!

From Flectra Online to on-premises
==================================

1. Log into `your Flectra Online user portal <https://accounts.flectra.com/my/databases/manage>`_ and look for the version number of your database.
2. If your database does not run a :ref:`major version <supported_versions>` of Flectra, you cannot host it on-premises yet, you have to upgrade it first to a new major version. (*e.g.: If your database runs Flectra 12.3 which is not a major version, you have to upgrade it first to Flectra 13.0 or 14.0.*)
3. Download a backup of your database by clicking on the "Gear" icon next to your database name then :menuselection:`Download` (if the download fails due to your backup file being too large, contact `our support <https://www.flectra.com/help>`_)
4. Restore it from the database manager on your local server.

From Flectra Online to Flectra.sh
=================================

1. Log into `your Flectra Online user portal <https://accounts.flectra.com/my/databases/manage>`_ and look for the version number of your database.
2. If your database does not run a :ref:`major version <supported_versions>` of Flectra, you cannot host it on Flectra.sh yet, you have to upgrade it first to a new major version. (*e.g.: If your database runs Flectra 12.3 which is not a major version, you have to upgrade it first to Flectra 13.0 or 14.0.*)
3. Download a backup of your database by clicking on the "Gear" icon next to your database name then :menuselection:`Download` (if the download fails due to your backup file being too large, contact `our support <https://www.flectra.com/help>`_)
4. Follow the :ref:`Import your database section of the Flectra.sh documentation <odoo_sh_import_your_database>`.

From Flectra.sh to Flectra Online
=================================

#. Uninstall all the **non-standard apps**.
#. `Create a support ticket <https://www.flectra.com/help>`_ and include the following:

   - Your subscription number
   - The URL you want to use for your database (e.g., `example.flectra.com`)
   - Which branch you want to migrate
   - In which region you want to be hosted:

     - Americas
     - Europe
     - Asia

   - Which user(s) will be the administrator(s)
   - When (and in which timezone) you want the database to be up and running

#. We will make sure your database is compatible and upload it to our cloud. In case of technical
   issues, we will get in touch with you.
#. All done!

.. important::
   - Flectra Online is not compatible with **non-standard apps**.
   - Make sure to uninstall all the **non-standard apps** in a staging build before doing it in your
     production build.

.. note::
   - Make sure you select the **region** that is closest to your users to reduce latency.
   - The future **administrator(s)** must have an flectra.com account.
   - The specific **date and time** at which you want the database to be up and running are mainly
     helpful to organize the switch from the flectra.sh server to the Flectra Online servers.
   - Databases are **not reachable** during their migration.
   - **If you have time constraints, contact us earlier to schedule the transfer**.

From Flectra.sh to on-premises
==============================

1.  Grab a :ref:`backup of your Flectra.sh production database <odoo_sh_branches_backups>`.
2.  Restore it from the database manager on your local server.
