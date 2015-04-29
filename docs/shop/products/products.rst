Add new products
================

Import products
---------------

The most efficient way to add new products is to import them via the csv
importer. To do so, you have to provide a valid csv file with your products.
In order to provide a valid data structure you have to map your csv headers
to our database properties. This is done by the importer widget. Simply add
your csv file and upload it.

.. hint:: Make sure to select the right encoding.

Once the file is uploaded the screen is changed to a mapper interface where
you can choose which of our database properties matches with your csv headers.

**Required fields are:**

* Productnumber
* Name
* Order unit
* Price

This is a very important step so please take your time for a careful mapping.
As this step takes quite some time we have created an intelligent mapping.
We try to indentify common mappings for you and preselect them in the interface.
And to make it even more convenient we will store your mapping, so once you
upload another file with new products you can reuse your personal mapping in
order to safe time.

Once you successfully have created the mapping, the csv file is ready to be
imported. However this is not done directly. As creating new products with all
their dependencies, e.g. media files, can take some time this import job is
passed to a `gearman worker <http://gearman.org/>`_ which starts to import your
products once the system is ready to do so. Once the import is finished an email
will be send to the email address defined in your sulu account and a reindex
script for elasticsearch will push your products to the elasticsearch index.

.. hint:: Images should always be uploaded before running the product import.

Add Product manually
--------------------

Adding a new product manually is very easy. Open your Sulu admin interface
and navigate to the *PIM* section. Add a new product and make sure you support
at least the required fields. Once you click save, the product is stored to the
database. There are two product states *activ* and *inactive* to choose if your
product should be visible in the shop or not.
