Sales-Order-Bundle
==================

Description
-----------

Bundle for handling sales orders.

Order PDF
---------

An order confirmation pdf can be downloaded by clicking the pdf icon in the
sidebar of any confirmed order in sulu's administration interface and will be
sent by email when a shop-order is made.
The PDF templates can be set in the configuration (see `Configuration`_ section
for further details).

Configuration
-------------

Default Configuration:

.. code-block:: yaml

    sulu_sales_order:
        pdf_templates:
            confirmation: SuluSalesOrderBundle:Pdf:order.confirmation.pdf.html.twig
            base: SuluSalesCoreBundle:Pdf:pdf-base.html.twig
            header: SuluSalesCoreBundle:Pdf:pdf-base-header.html.twig
            footer: SuluSalesCoreBundle:Pdf:pdf-base-footer.html.twig
            macros: SuluSalesCoreBundle:Pdf:pdf-macros.html.twig
        shop_email_from: null
        shop_email_confirmation_to: null
        send_email_confirmation_to_customer: true
        send_email_confirmation_to_shopowner: true

pdf_templates
~~~~~~~~~~~~~

Define the templates to use for pdf generation.

shop_email_from
~~~~~~~~~~~~~~~

Emailaddress of the sender of all confirmation emails.

shop_email_confirmation_to
~~~~~~~~~~~~~~~~~~~~~~~~~~

Email address of shop-owner. This is the address on which the shop owner will be notified if an order has been made.

send_email_confirmation_to_customer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Defines if an email confirmation should be sent to the customer after submitting an order.
send_email_confirmation_to_shopowner
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Defines if an email confirmation should be sent to the shopowner.
