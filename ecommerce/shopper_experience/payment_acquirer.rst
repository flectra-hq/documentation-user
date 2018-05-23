===================================================
How to manage orders paid with payment acquirers
===================================================

Flectra confirms orders automatically as soon as the payment is authorized 
by a payment acquirer. This triggers the delivery.
If you invoice based on ordered quantities,
you are also requested to invoice the order.


What are the payment status
===========================
At anytime, the salesman can check the transaction status from the order.

.. image:: media/payment_transaction.png
    :align: center

* *Draft*: transaction under processing.

* *Pending*: the payment acquirer keeps the transaction on hold and you 
  need to authorize it from the acquirer interface.

* *Authorized*: the payment has been authorized but not yet captured.
  In Flectra, the order is already confirmed. Once the delivery done, you
  can capture the amount from the acquirer interface (or from Flectra if you use
  Authorize.net).

* *Done*: the payment is authorized and captured. The order has been confirmed.

* *Error*: an error has occured during the transaction. 
  The customer needs to retry the payment.
  The order is still in draft.

* *Cancelled*: when the customer cancels the payment in the payment acquirer form.
  They are taken back to Flectra in order to modify the order.

.. note:: Specific messages are provided to your customers for every
   payment status, when they are redirected to Flectra after the transaction.
   To edit such messages, go to the *Messages* tab of the payment
   method.
