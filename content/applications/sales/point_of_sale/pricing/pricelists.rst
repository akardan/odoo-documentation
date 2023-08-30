==========
Pricelists
==========

The pricelist feature allows you to adjust product prices based on predefined criteria.

It can be used for a designated duration, like a temporary sale on products within a particular PoS
category, for specific users, or as a reward when customers meet certain conditions, such as a
minimum purchase quantity or amount.

Configuration
=============

To **activate** the pricelist feature, access the :ref:`general PoS app's settings
<configuration/settings>` and enable :guilabel:`Pricelists` in the :guilabel:`Pricing` section.

Then, select the :ref:`type of pricelist <pricelists/create>` by checking :guilabel:`Multiple prices
per product` or :guilabel:`Advanced price rules (discounts, formulas)`, save, and click
:guilabel:`Pricelists` to create new ones or modify existing ones.

.. image:: pricelists/settings.png
   :alt: enabling the pricelists feature in the general PoS' settings.

.. note::
   Alternatively, you can go to :menuselection:`Point of Sales --> Products --> Pricelists` to reach
   the previous screen.

.. _pricelists/create:

Create pricelists
=================

Click :guilabel:`Create` or select an existing pricelist. The pricelist setup form differs depending
on the chosen type of pricelist.

.. tabs::
   .. tab:: Multiple prices per product

      This type of pricelist requires selecting a product to which you can attribute one or
      multiple other prices. To do so,

      #. click :guilabel:`Add a line` and select a product;
      #. add conditions such as a specific quantity to reach for the price to change in the
         :guilabel:`Min. Quantity` column or a determined period during which the pricelist
         can be applied in the :guilabel:`Start Date` and :guilabel:`End Date` columns;
      #. filter the pricelist to be set on one specific variant of the selected product in the
         :guilabel:`Variants` column.

      .. image:: pricelists/multiple-prices.png
         :alt: setup form of a multiple prices pricelist.

      .. note::
         - Conditions and filters are optional. You can leave these columns empty to use a pricelist
           without conditions.
         - Pricelists can be set on a POS order if the conditions are unmet, but the computation
           will not be applied.

   .. tab:: Advanced price rules

      To set up this type of pricelist:

      #. Click :guilabel:`Add a line` and select one of the three available computations in the
         pop-up window:

         - :guilabel:`Fixed Price` to attribute another price to the designated product(s).
         - :guilabel:`Discount` to attribute a discount to the designated product(s).
         - :guilabel:`Formula` to compute the prices according to a formula that combines
           multiple computations:

           - Define what the calculation is based on (the :guilabel:`Sales Price`, the
             :guilabel:`Cost`, or an :guilabel:`Other Pricelist`.)
           - Apply a :guilabel:`Discount` and/or add an :guilabel:`Extra Fee`.
           - Define a :doc:`Rounding Method <cash_rounding>` and specify the minimum amount of
             **margin** over the base price *(optional)*.

      #. Select the products you want to apply this computation to:

         - :guilabel:`All Products`
         - a :guilabel:`Product Category`
         - a specific :guilabel:`Product`
         - a specific :guilabel:`Product Variant`

      #. Add conditions, such as a specific quantity to reach for the price to change in the
         :guilabel:`Min. Quantity` field or a specific period of time during which the pricelist can
         be applied in the :guilabel:`Validity` fields.

      .. image:: pricelists/price-rules.png
         :alt: setup form to configure an advanced pricelist

      .. note::
         Pricelists can be set on a POS order if the conditions are unmet, but the computation will
         not be applied.

Once pricelists are created, go to the :ref:`POS settings <configuration/settings>` and select
either one pricelist in the :guilabel:`Default Pricelist` field or tick the :guilabel:`Advanced
Pricelists` checkbox and fill in the :guilabel:`Available` field with all the desired pricelists.

.. note::
   - All available pricelists must be in the same currency as the company or the **Sales Journal**
     set on the selected point of sale.
   - Changes to the pricelist feature setup affect the entire database and also apply to the
     :doc:`Sales <../../sales/products_prices/prices/pricing>` and :ref:`eCommerce
     <multi_website/pricelists>` apps.

Use pricelists
==============

:ref:`Open a POS session <pos/session-start>`, click the **pricelists** button, and select the
desired pricelist from the list.

.. image:: pricelists/pricelist-button.png
   :alt: button to select a pricelist on the pos frontend

You can also set a pricelist to be selected automatically once a specific :ref:`customer is set
<pos/customers>`. To do so, go to the customer form and switch to the preferred pricelist in the
:guilabel:`Pricelist` field of the :guilabel:`Sales & Purchase` tab.

.. note::
   Multiple pricelists must be selected for the **pricelist button** to be displayed.

.. seealso::
   - :doc:`../../sales/products_prices/prices/pricing`
   - :ref:`How to use pricelists in a multi-website environment <multi_website/pricelists>`
