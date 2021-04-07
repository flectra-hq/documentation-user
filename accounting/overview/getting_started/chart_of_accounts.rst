=================
Chart of Accounts
=================

The **Chart of Accounts (COA)** is the list of all the accounts used to record financial
transactions in the general ledger of an organization.

The accounts are usually listed in the order of appearance in the financial reports. Most of the
time, they are listed as follows :

- Balance Sheet accounts

  * Assets
  * Liabilities
  * Equity

- Profit & Loss

  * Income
  * Expense

When browsing your Chart of Accounts, you can filter the accounts by number, in the left column, and
also group them by Account Type.

.. image:: media/chart_of_accounts01.png
   :align: center
   :alt: Group the accounts by type in Flectra Accounting

Configuration of an Account
===========================

The country you select at the creation of your database (or additional company on your database)
determines which **Fiscal Localization Package** is installed by default. This package includes a
standard Chart of Accounts already configured according to the country's regulations. You can use
it directly or set it according to your company's needs.

.. warning::
   It is not possible to modify the **Fiscal Localization** of a company once a Journal Entry has
   been posted.

To create a new account, go to :menuselection:`Accounting --> Configuration --> Chart of Accounts`,
click on *Create*, and fill out the form.

Code and Name
-------------

Each account is identified by its **Code** and **Name**, which also indicates the account's purpose.

Type
----

Configuring correctly the **Account Type** is critical as it serves multiple purposes:

- Information on the account's purpose and behavior
- Generate country-specific legal and financial reports
- Set the rules to close a fiscal year
- Generate opening entries

To configure an account type, open the **Type** field's drop-down selector and select the right
type among the following list:

+---------------+--------------+-------------------------+
| Report        | Category     | Account Types           |
+===============+==============+=========================+
| Balance Sheet | Assets       | Receivable              |
|               |              +-------------------------+
|               |              | Bank and Cash           |
|               |              +-------------------------+
|               |              | Current Assets          |
|               |              +-------------------------+
|               |              | Non-current Assets      |
|               |              +-------------------------+
|               |              | Prepayments             |
|               |              +-------------------------+
|               |              | Fixed Assets            |
|               +--------------+-------------------------+
|               | Liabilities  | Payable                 |
|               |              +-------------------------+
|               |              | Credit Card             |
|               |              +-------------------------+
|               |              | Current Liabilities     |
|               |              +-------------------------+
|               |              | Non-current Liabilities |
|               +--------------+-------------------------+
|               | Equity       | Equity                  |
|               |              +-------------------------+
|               |              | Current Year Earnings   |
+---------------+--------------+-------------------------+
| Profit & Loss | Income       | Income                  |
|               |              +-------------------------+
|               |              | Other Income            |
|               +--------------+-------------------------+
|               | Expense      | Expense                 |
|               |              +-------------------------+
|               |              | Depreciation            |
|               |              +-------------------------+
|               |              | Cost of Revenue         |
+---------------+--------------+-------------------------+
|Other          | Other        | Off-Balance Sheet       |
+---------------+--------------+-------------------------+

Assets, Deferred Expenses, and Deferred Revenues Automation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Some Account Types display a new field **to automate** the creation of :ref:`Assets
<assets-automation>` entries, :ref:`Deferred Expenses <deferred-expenses-automation>` entries,
and :ref:`Deferred Revenues <deferred-revenues-automation>` entries.

You have three choices for the **Automation** field:

#. **No:** this is the default value. Nothing happens.
#. **Create in draft:** whenever a transaction is posted on the account, a draft entry is created,
   but not validated. You must first fill out the corresponding form.
#. **Create and validate:** you must also select a Model. Whenever a transaction is posted on the
   account, an entry is created and immediately validated.

.. note::
   Please refer to the related documentation for more information.

Default Taxes
-------------

Select a **default tax** that will be applied when this account is chosen for a product sale or
purchase.

Tags
----

Some accounting reports require **tags** to be set on the relevant accounts. By default, you can
choose among the tags that are used by the *Cash Flow Statement*.


.. seealso::
   * :doc:`../../payables/supplier_bills/assets`
   * :doc:`../../payables/supplier_bills/deferred_expenses`
   * :doc:`../../receivables/customer_invoices/deferred_revenues`
   * :doc:`../../fiscal_localizations/overview/fiscal_localization_packages`