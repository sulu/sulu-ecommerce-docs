Shopping Cart
=============

Cart widget
-----------

The cart widget allows a user to put a product into the shopping cart. The widget
consists of an input field for the quantity and a button to finally add it.
Quantity must be a valid number, therefore this field is validated. If an invalid
input is made a discreet error is displayed. Default quantity is one. So if the
button is clicked without any other action, one product is added to the shopping
cart.

Cart display widget
-------------------

This widget is used to display what is currently in the cart. Behind the scenes
it triggers an ajax call to get the shopping cart information. It then displays
the current total sum and the amount of product items in the shopping cart.

Cart detail page
----------------

The shopping cart detail page gives an overview for all products in the cart. It
is possible to increase or decrease the quantity of a specific product, change
the invoice and shipping address or if a product got accidentally into the cart,
remove it. Also the total prices and the shipping costs are properly displayed.
As an user can have exactly one cart, the current cart content is stored for later
reuse. Once the order is completed, the shopping cart is emptied and a success
screen is shown to the user. A permanent url endpoint for the detail page exists
and can be opened manually via ``/shoppingcart``.
