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
            base: SuluSalesCoreBundle:Pdf:pdf-base.html.twig
            header: SuluSalesCoreBundle:Pdf:pdf-base-header.html.twig
            footer: SuluSalesCoreBundle:Pdf:pdf-base-footer.html.twig
            macros: SuluSalesCoreBundle:Pdf:pdf-macros.html.twig

