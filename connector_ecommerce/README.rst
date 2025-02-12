========================
Connector for E-Commerce
========================

.. 
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! source digest: sha256:49ddd28c8d1b54bef16f9026aa5a6add6d88ab26a9bc72180e46849633302f56
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fconnector--ecommerce-lightgray.png?logo=github
    :target: https://github.com/OCA/connector-ecommerce/tree/16.0/connector_ecommerce
    :alt: OCA/connector-ecommerce
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/connector-ecommerce-16-0/connector-ecommerce-16-0-connector_ecommerce
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
    :target: https://runboat.odoo-community.org/builds?repo=OCA/connector-ecommerce&target_branch=16.0
    :alt: Try me on Runboat

|badge1| |badge2| |badge3| |badge4| |badge5|

This modules aims to be a common layer for the connectors dealing with
e-commerce.

It sits on top of the `connector`_ framework and is used by the
e-commerce connectors, like `magentoerpconnect`_ or
`prestashoperpconnect`_.

That's a technical module, which include amongst other things:

Events

  On which the connectors can subscribe listeners.
  The events it adds are:

   * ``on_invoice_paid(self, record)``
   * ``on_invoice_validated(self, record)``
   * ``on_invoice_validated(self, record)``
   * ``on_picking_out_done(self, record, method)`` where method is
     'partial' or 'complete'
   * ``on_tracking_number_added(self, record)``
   * ``on_product_price_changed(self, record)``

 Components

  A piece of code which allows to play all the ``onchanges`` required
  when we create a sales order.

  Another one which allows to add special lines in imported sales orders
  such as Shipping fees, Cash on Delivery or Discounts.

Data Model

  Add structures shared for e-commerce connectors

.. _`connector`: http://odoo-connector.com
.. _`magentoerpconnect`: http://odoo-magento-connector.com
.. _`prestashoperpconnect`: https://github.com/OCA/connector-prestashop

**Table of contents**

.. contents::
   :local:

Installation
============

This module is a dependency for more advanced connectors. It does
nothing on its own and there is no reason to install it alone.

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/connector-ecommerce/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us to smash it by providing a detailed and welcomed
`feedback <https://github.com/OCA/connector-ecommerce/issues/new?body=module:%20connector_ecommerce%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* Camptocamp
* Akretion

Contributors
~~~~~~~~~~~~

See `contributors <https://github.com/OCA/connector-ecommerce/graphs/contributors>`_.

Other credits
~~~~~~~~~~~~~

The migration of this module from 13.0 to 14.0 was financially supported by Camptocamp.

Maintainers
~~~~~~~~~~~

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

This module is part of the `OCA/connector-ecommerce <https://github.com/OCA/connector-ecommerce/tree/16.0/connector_ecommerce>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
