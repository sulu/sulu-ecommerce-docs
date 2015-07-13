Product search
==============

How it works
------------

The product search is based on elasticsearch. This means all searchable products
must be indexed. The search API is split in two main parts. There is a live search
api which provides functionallity to be used in e.g. a typeahead. The main search
lists all products which match for a given query string. This result can also be
filtered by additional information such as the category or the supplier.

Configuration
-------------

Each product consitsts of multiple properties e.g. title, description, categories.title
and so on. The fields that has to be considered for a search must be defined as list under
the 'search_fields' section in the `config.yml`. Additionaly it's possible to define a weight, which
indicates the relevance for the specific field among the other fields for the search result.
To increase the boost for an appropriate property it can be postfixed with '^' followed by a
number (factor).

It is also possible to add additional term queries to the search.

An example of a valid configuration is given below::

    bundle_name:
        search_fields:
            - title^10
            - description^5
            - categories.title
        term_queries:
            - {field: isContractArticle, value: true, parameters: {boost: 0.5}, type: 'should'} 

Search widget
-------------

The search widget is one of the main parts of each shop. It helps the user to
find products and more. If the user starts typing, additional ajax requests are
placed in the background asynchronously to display suggestions. Once you click on
a suggestion, you are redirected to the product detail page. If you just type in
a query string and hit enter, a fulltext search is placed and matching products
are returned in a batched list.

Prefilter Categories
--------------------

Sometimes it makes sense to search a product within a certain category only. For
example it would make propably no sense to search a fridge within sporting goods.
Nor you want loads of other products to be found if you already know what you are
looking for. Therefore it is possible to select a category and prefilter the
search results.
