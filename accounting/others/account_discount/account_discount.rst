=================================
How to work with Account Discount
=================================

Introduction
============

The document is about how the discount which is to be applied over Invoice.

It is an advance discounting system, where the user can set limit in
provision of discount.

-   There are two ways of configuring Discount.

    1.  Global Discount
    2.  Ordinary Discount

Fixed discount amount and Percentage discount will be applied on Invoice lines discount.

Configurations / Settings
=========================

How to configure Global Discount
--------------------------------

To configure Global Discount, goto :menuselection:`Invoicing --> Configuration --> Settings`.

.. image:: ./media/global_settings.png

Once the user configures Global Discount, the discount will be applied
every where in Invoice upto the configured discount amount
and percentage.

If user marks the 'Global Discount', there will be a checkbox shown
with the confirmation message 'Do you want to set global discount limit?'.
Marking that checkbox, There will be two fields, which takes user of discount
limits in Fix Amount and Percentage.

How to configure Ordinary Discount
----------------------------------

To configure Ordinary Discount, goto :menuselection:`Invoicing --> Configuration --> Accounting --> Discounts.`

.. image:: ./media/ordinary_discount.png

.. note::
    Here, the user has to set a group and its discount limits in Fix Amount
    and Percentage.

Working with Discounts
======================

Account Discounts
-----------------

In Account Discounts, the user is supposed to configure discount amount and
percentage against user groups.

The user will not be able to configure the discount amount and percentage more
than defined in the Settings, and will raise an error message.

.. image:: ./media/validation_error.png
    :align: center

Discounts over Invoices
-----------------------

-   **Discount Percentage**

.. note::
    As the user configures Global Discount, the ordinary discount cannot be
    exceeded than Global Discount.

.. image:: ./media/invoice.png
    :align: center

Discount will be applied either in percentage or in fixed amount.

If the discount method is in percentage, select the Discount method 'Percentage',
and fill in Discount(%) filed from 1 to 100. To apply the discount, there is button
below the Discount labeled as '(Update Discount)'.

.. image:: ./media/update_discount.png

.. note::
    If the discount percentage exceeds than the configured discount percentage, then
    error message will be raised.

.. image:: ./media/exceed_error.png

Before applying the discount over the Invoice lines, the system will ask for confirmation.
It will apply the percentage in all the Invoice lines under discount column.

.. image:: ./media/confirm_update.png

.. note::
    In invoice, if the method is Percentage, then the percentage will be applied in
    each line of the invoice.

-   **Fixed Discount Amount**

Select the discount method 'Fixed' and fill in Discount Amount field. If user
applies the discount by clicking on '(Update Discount)', the given amount will
be divided amount all Invoice Lines, and the percentage will be calculated
according to the amount.

.. image:: ./media/line_discount.png
    :align: center
