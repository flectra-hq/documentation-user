=====================
Easypost Shipping API
=====================

EasyPost is a software company that helps businesses integrate shipping from the major carriers. It has accross 60+ carriers. To start working with Easypost, you need to install easypost api(sudo apt-get install easypost).

Get Credentials
---------------

Login into the dashboard of Easypost. Easypost will provide you API KEY.

.. image:: media/easy-1.png
    :align: center


Carrier Account ID
------------------

You will get the carrier account ID from the Easypost Dashboard.
Go to :menuselection:`My Profile --> Carrier Accounts`.

.. image:: media/easy-2.png
    :align: center

Easypost Configuration
----------------------

Delivery method name should be delivery carrier name and the package name.

If your easypost carrier account support the scanform then tick the ScanForm Supported.

Go to :menuselection:`Inventory --> Configuration --> Shipping Methods`..

.. image:: media/easy-3.png
    :align: center

Sale Order
----------

Create new Sale Order and Select the delivery method, you will get the carrier rates of the items. Easypost also supports multi currency.

Note:Address should be correct. 

.. image:: media/easy-4.png
    :align: center

Get Label in attachment
-----------------------

After confirming Sale Order, click on :menuselection:`Delivery --> Validate --> Apply`, you will get the label url in attachment.

.. image:: media/easy-5.png
    :align: center

Shipment Label
--------------

Shipment Label In Attachment 

.. image:: media/easy-6.png
    :align: center

Retrieve Label
--------------

If the label is deleted, you can retrieve it by clicking on `Retrieve Label`. 

.. image:: media/easy-5.png
    :align: center

Tracking URL
------------

Click on Tracking, you will get the tracking url. 

.. image:: media/easy-7.png
    :align: center

Get Tracking Details
--------------------

Click On `Tracker Details` to get the tracker status updated. Also a schedulers runs after every minute Which update the status and other details.

.. image:: media/easy-8.png
    :align: center

Get Shipping ID
---------------

Create new Scanform. Select the starting and ending date.Click on Get Shipping ID, you will get the list of Shipping IDS.
Note:The shipping Ids which are already manifested or whose labels are remaining to create will not be shown. 

.. image:: media/easy-9.png
    :align: center

Create Batch and Scanform
-------------------------

Click on Create Batch And Scanform. Batch ID and Scanform ID will be generated. 

.. image:: media/easy-10.png
    :align: center

Postage Label
-------------

You will get the postage label in attachment while creating Batch and ScanForm.

.. image:: media/easy-11.png
    :align: center

