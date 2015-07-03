Shop Customer Settings
======================

Basic information about the shop owner is often used within templates and various
other documents such as PDFs. To add and edit them centrally there is a config
file located at `app/config/shopowner.yml`. It can be enhanced as needed.
Be careful with deleting properties from this file and make sure you edit it
carefully.

A basic config eg. looks like this

.. code-block:: yaml

    parameters:
        shopowner:
            name: 'My Great Company Ldt'
            name_short: 'MGC'
            name_addition: 'Ldt'
            slogan: 'Create a better world'
            website: 'www.mgc.com'
            company_uid: 'ATU 123456'
            company_register: '315317b'
            phone: '+43 1111 220 20-0'
            fax: '+43 1111 220 20-106'
            address:
                street: 'Mystreet'
                number: '6'
                zip: '6850'
                city: 'Dornbirn'
                country: 'Austria'
            bank:
                name: 'Hypobank Dornbirn'
                iban: 'AT20 1100 2200 3300 4400'
                bic: 'HYPVAT2B'
            email:
                office: 'office@mgc.com'

