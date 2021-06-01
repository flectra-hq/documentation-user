===================================
Manage a bank in a foreign currency
===================================

In Flectra, every transaction is recorded in the default currency of the
company. Reports are all based on the currency of the company. But for
transactions occurring in another currency, Flectra stores both the value
in the currency of the company and the value in the currency of the
transaction.

When you have a bank account in a foreign currencies, for every
transaction, Flectra stores two values:

-  The debit/credit in the currency of the company

-  The debit/credit in the currency of the bank account

Currency rates are updated automatically using yahoo.com, or the
European Central bank web-services.

Configuration
==============

Activate the multi-currency feature
-----------------------------------

In order to allow your company to work with multiple currencies, you
should activate the multi-currency mode. In the accounting application,
go into :menuselection:`Configuration --> Settings --> Accounting & Finance Features`
make sure the **Allow Multi-currencies** box is ticked. Provide
a **Currency Exchange Gain / Loss** account, then click on **Apply**.

Configure currencies
--------------------

Once the Flectra is configured to support multiple currencies, you should
activate the currencies you plan to work with. To do that, go to the menu
:menuselection:`Configuration --> Currencies`. All the currencies are created by default,
but you should activate the ones you plan to support (to activate a
currency, check its "Active" field).

After having activated the currencies, you can configure the parameters
to automate the currency rate update. These options are also in the
settings of the Accounting application, in the bottom of the page:

