Submitting an order
===================

Confirmation Emails
-------------------

When an order is submitted an email is sent

* to **the customer** and
* to **the shop owner**

.. hint:: Both emails have the **order-confirmation pdf** attached.

Who is receiving the order confirmation?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Customer
~~~~~~~~

On the customers side the email will be sent to the person who makes the order.

Shop Owner
~~~~~~~~~~

On the shop owners side, the email is sent to

* the **responsible person** of the customers company (if defined)
* OR to the email-address which is defined as **order-confirmation address in the config**


Define Email Text
^^^^^^^^^^^^^^^^^

The easiest way to change the content of the emails is to override the translations, which are defined in
``[SuluSalesOrderBundle]/Resources/translations/order_confirmation_email.[LANGUAGE].xlf``
