==============================
 Debt/Credit notebook for POS
==============================

The module allows to make sale on credit.

Debt (Credit) value is changed whenever:

* Product marked as "Credit Product" is sold via POS or via Invoices. Invoices created via website_sale (eCommerce) module are supported too.
* POS payment is made via journal marked as "Debt journal"
* "Manual Credit Updates" is added

Other features:

* each user has Debt Limit field. By default is 0, i.e. user has to pay in advance and cannot have negative credits amount.

Installation \ Deinstallation
=============================

* Debt data are still available after the module will be re-installed.
* When new (first after install) POS session is opened, a debt payment method would added in a POS config.
* If the module was install and uninstall immediately (without created POS sessions) then it keeps no data.   
* If a user deleted debt journal from POS config manually then after the module is upgraded 
  POS config would not be changed. 
* Multicompany mode is supported

Credits
=======

Contributors
------------
* krotov@it-projects.info

Sponsors
--------
* `IT-Projects LLC <https://it-projects.info>`__

Further information
===================

Demo: http://runbot.it-projects.info/demo/pos-addons/9.0

HTML Description: https://apps.odoo.com/apps/modules/9.0/pos_debt_notebook/

Usage instructions: `<doc/index.rst>`__

Changelog: `<doc/changelog.rst>`__

Tested on Odoo 10.0 8bd56bb46628e57f41c635f20c527264d7a20d86
