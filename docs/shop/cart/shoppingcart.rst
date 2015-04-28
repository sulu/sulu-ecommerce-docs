Shopping Cart
=============

Cart widget
-----------

The cart widget allows a user to put a product into the shopping cart. The widget
consists of an input field for the quantity and a button to finally add it.
Quantity must be a valid number therefore this field is validated. If an invalid
input is made a dezent error is displayed. Default quantity is one.

Cart detail page
----------------

The shopping cart detail page gives an overview for all products in the cart. It
is possible to increase or decrease the quantity of a specific product, change
the invoice and shipping address or if a product got accidentally into the cart,
remove it. Also the total prices and the shipping costs are well displayed.
As a user can have one cart only, the current cart content is stored for later
reuse. Once the order is completed, the shopping cart is emptied and a success
screen is shown to the user. A permanent url endpoint for the detail page exists
and can be opened manually via ``/shoppingcart``.
