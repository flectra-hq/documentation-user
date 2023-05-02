.. _developer-mode:

===========================
Developer Mode (debug mode)
===========================

The developer mode (or debug mode) unlocks access to extra and advanced tools in Flectra. There are
several ways to activate the developer mode: through the

.. _general/developer_mode/settings:

Activate through the Settings
=============================

The debug mode can be activated in the Flectra database settings. Go to :menuselection:`Settings -->
General Settings --> Developer Tools` and click on :guilabel:`Activate the developer mode`. At
least one application needs to be installed for the :guilabel:`Developer Tools` section to appear
in the :guilabel:`Settings` module.

.. image:: developer_mode/settings.png
   :align: center
   :alt: Overview of the debug options under settings in Flectra.

.. note::
   :guilabel:`Activate the developer mode (with assets)` is used by developers; :guilabel:`Activate
   the developer mode (with tests assets)` is used by developers and testers.

Once activated, the :guilabel:`Deactivate the developer mode` option becomes available.

.. _general/developer_mode/browser-extension:

Activate through the browser extension
======================================

Within a web browser, navigate to the browser settings and extensions and search for the `Flectra
Debug` extension. Once the extension is installed, a new icon will be shown on the browser's
toolbar.

For the *Flectra Debug* extension, a single click enables a normal version of the mode, while a
double click enables it with assets. To deactivate it, use a single click.

Activate through the URL
========================

The debug mode can also be activated by adding an extra query string to the database's URL. In the
URL, add `?debug=1` or `?debug=true` after `/web`. To deactivate the debug mode, change the
value to `?debug=0` instead.

.. image:: developer_mode/url.png
   :align: center
   :alt: Overview of a URL with the debug mode command added.

.. tip::
   Additional modes are available for developers: `?debug=assets` enables the
   :ref:`assets mode <frontend/framework/assets_debug_mode>`, and `?debug=tests` enables
   the :ref:`tests mode <frontend/framework/tests_debug_mode>`.

.. _developer-mode/mode-tools:

Locate the developer mode tools
===============================

Once developer mode is activated, the developer mode tools can be accessed from the :guilabel:`Open
Developer Tools` button, the bug icon located in the header of the Flectra database.

.. image:: developer_mode/button-location.png
   :align: center
   :alt: Overview of a console page and the debug icon being shown in Flectra.

This menu contains additional tools that are useful to understand or edit technical data, such as
the views or actions of a page. On a page that has filters, actions, and view options, the
developer mode tools contain some useful menu items such as:

- :guilabel:`Edit Action`
- :guilabel:`Manage Filters`
- Edit the current view (e.g. Kanban, List, Graph, etc.)
- See the :guilabel:`Fields View Get`
