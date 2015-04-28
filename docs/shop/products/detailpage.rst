Product detail page
===================

How to reach it
---------------

All product detail pages can be opened by browsing ``/products/<productId>``.
This is the permanent product url. It will be extended by the urlencoded product
title in order to improve the seo behavoir of the shop.

Product details
---------------

The basic product details are shown on the detail page such as title, short and
long description, product number, existing product attributes. These information
are fetched by the database as it is very important to display the real up to
date data to the user.

Image gallery
-------------

There is an image gallery on the detail page to display all given product images.
Default the first image is displayed as a large cover image. For all images there
is a thumbnails beyond the cover image. By clicking on it the thumbnail is
switching place with the cover image. By moving the mouse over the cover image
it is zoomed in if the image is large enough. If no image exists a fallback image
is displayed which is not zoomable.

Ratings box
-----------

The ratings box shows the product rating based on all rates been given for this
product and a link to customer reviews. Each user is allowed to rate a product
once.

Supplier box
------------

The supplier is displayed on the detail page. All important information is shown
such as the name, the address and the contact data.

Cart widget - prices
--------------------

All product detail pages provide the cart widget which enables the user to add a
certain product to his shopping cart. The cart widget also displays the product
prices. Prices means that there is generally a basic price, however there could
also be a scale price.

Check the :doc:`../cart/shoppingcart` section for more information.

Other supplier widget
---------------------

As many different suppliers can offer the same product, there is a *other supplier*
widget to show the user some more offers for the same product. To detect identical
products a product must provide a global trading number. To improve the loading
speed and the query time this list is provided by elasticsearch.

Similar products widget
-----------------------

To help the user find more products he might be interested in there is a very
useful widget which displays a similar prodcuts list. This feature is implemented
by an *elasticsearch more like this* query which compares the current product
with other products in the index. If products with a similarity are detected they
are returned and displayed.
