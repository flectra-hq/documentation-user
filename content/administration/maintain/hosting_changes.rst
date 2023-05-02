
.. _db_management/hosting_changes:

=======================
Change hosting solution
=======================

You may want to move your Flectra database from one hosting solution to another.
Depending on the platforms, you have to do it by yourself or contact our support team first.

From on-premises to Flectra Online
==================================

1. Grab a "dump with filestore" of your database by using the Database Manager.
2. **If you have time constraints, contact us earlier to schedule the transfer.**
3. `Create a support ticket <https://www.flectrahq.com/help>`_ and attach the dump (if the file is too large, use any file transfer service and attach the link to your ticket). Also include your subscription number and the URL you want to use for your database (e.g.: my-company.flectra.com).
4. We will make sure your database is compatible and upload it to our cloud. In case of technical issues, we will get in touch with you.
5. It's done!

.. important::
   - Flectra Online is not compatible with **non-standard apps**.
   - The database you are moving to Flectra Online must be in a :doc:`supported version
     <supported_versions>`.


#. Uninstall all the **non-standard apps**.
#. `Create a support ticket <https://www.flectrahq.com/help>`_ and include the following:

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
