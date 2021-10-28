
.. _db_management/hosting_changes:

===============
Hosting Changes
===============

You may want to move your Flectra database from one hosting solution to another.
Depending on the platforms, you have to do it by yourself or contact our support team first.

From on-premises to Flectra Online
==================================

.. warning:: Flectra Online is not compatible with **non-standard apps**.

1. Create a :ref:`duplicate <duplicate_premise>` of your database: in this duplicate, uninstall all the **non-standard apps**.
2. Grab a "dump with filestore" of your database by using the Database Manager.
3. **If you have time constraints, contact us earlier to schedule the transfer.**
4. `Create a support ticket <https://www.flectrahq.com/help>`_ and attach the dump (if the file is too large, use any file transfer service and attach the link to your ticket). Also include your subscription number and the URL you want to use for your database (e.g.: my-company.flectrahq.com).
5. We will make sure your database is compatible and upload it to our cloud. In case of technical issues, we will get in touch with you.
6. It's done!

From Flectra Online to on-premises
==================================

1. Log into `your Flectra Online user portal <https://accounts.flectrahq.com/my/databases/manage>`_ and look for the version number of your database.
2. If your database does not run a :ref:`major version <supported_versions>` of Flectra, you cannot host it on-premises yet, you have to upgrade it first to a new major version. (*e.g.: If your database runs Flectra 12.3 which is not a major version, you have to upgrade it first to Flectra 13.0 or2.0.*)
3. Download a backup of your database by clicking on the "Gear" icon next to your database name then :menuselection:`Download` (if the download fails due to your backup file being too large, contact `our support <https://www.flectrahq.com/help>`_)
4. Restore it from the database manager on your local server.

.. warning:: Flectra Online is not compatible with **non-standard apps**.

1.  Uninstall all the **non-standard apps**: test it in a staging build first, then do it in your production build.
2.  **If you have time constraints, contact us earlier to schedule the transfer.**
3. `Create a support ticket <https://www.flectrahq.com/help>`_ and attach the dump (if the file is too large, use any file transfer service and attach the link to your ticket). Also include your subscription number and the URL you want to use for your database (e.g.: my-company.flectrahq.com).
4.  We will make sure your database is compatible and upload it to our cloud. In case of technical issues, we will get in touch with you.
5.  It's done!


