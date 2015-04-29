Product list
============

Where does the data come from
-----------------------------

To provide best performance the product list is provided by elasticsearch.
Therefore only products which are in the current index can be found in the list.
To increase the applicability of the list, the basic function to get products is
a high generalized elasticsearch search function which can be used in many
different ways. Since always the same data structure is returned by the
elasticsearch layer, we can provide a high level of consistency.

The default list
----------------

The default list provides a batched search result where each item represents a
real product. The following information is shown if exists:

* Title
* Short description
* Image
* Price
* Price per order unit
* Global Trading Number (GTIN, EAN)
* Product ratings

A click on a single item leads to the product detail page.

Usage
-----

Currently product lists are shown at:

* Filtered products for category navigation
* Filtered products for live product search
* List for other suppliers for a specific product
* List for similar products
