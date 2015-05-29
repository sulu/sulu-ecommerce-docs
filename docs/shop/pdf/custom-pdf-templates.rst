Custom Order Confirmation PDF Templates
=======================================

Defining a custom order-confirmation pdf template is really easy. First define
your twig templates as you usually would. This can be done for the

- confirmation
- header
- footer
- base and
- macros


Header and footer are shown - as you probably already expected - at the top and
the bottom of every page.
The 'base' template is defining the general content of your order-pdf,
like introduction, headline of you pdf and so on.
It should contain the following blocks if you'd like it to show all the
possible information provided by an order:

- company_slogan
- recipient_business_info
- recipient
- responsibleperson
- pdf_title
- invoice_address
- orderdetails
- shippingdetails
- shippingdetails_addressnote_title
- shippingdetails_addressnote_content
- productlist
- productlist_items
- productlist_footer_shippingcost_title
- productlist_footer_total_title
- productlist_footer_shippingcost_value
- productlist_footer_total_value

In the 'confirmation' file you can define blocks of an order-confirmation.
The 'macros' template contains macro functionality e.g. for displaying the
items.



