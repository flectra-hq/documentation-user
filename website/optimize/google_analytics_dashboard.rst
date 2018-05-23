=============================================================
How to track your website traffic from your Flectra Dashboard
=============================================================

You can follow your traffic statistics straight from your Flectra Website 
Dashboard thanks to Google Analytics.

- A preliminary step is creating a Google Analytics account and entering the 
  tracking ID in your Website's settings (see :doc:`google_analytics`).

- Go to `Google APIs platform <https://console.developers.google.com>`__ 
  to generate Analytics API credentials. Log in with your Google account. 

- Select Analytics API.

.. image:: media/google_analytics_api.png
    :align: center

- Create a new project and give it a name (e.g. Flectra).
  This project is needed to store your API credentials.

.. image:: media/google_analytics_create_project.png
    :align: center

- Enable the API.

.. image:: media/google_analytics_enable.png
    :align: center

- Create credentials to use in Flectra.

.. image:: media/google_analytics_create_credentials.png
    :align: center

- Select *Web browser (Javascript)* 
  as calling source and *User data* as kind of data.

.. image:: media/google_analytics_get_credentials.png
    :align: center

- Then you can create a Client ID.
  Enter the name of the application (e.g. Flectra) and the allowed pages on 
  which you will be redirected. The *Authorized JavaScript origin* is your 
  Flectra's instance URL. The *Authorized redirect URI* is your Flectra's instance 
  URL followed by '/google_account/authentication'.

.. image:: media/google_analytics_authorization.png
    :align: center


- Go through the Consent Screen step by entering a product name 
  (e.g. Google Analytics in Flectra). Feel free to check the customizations options 
  but this is not mandatory. The Consent Screen will only show up when you enter 
  the Client ID in Flectra for the first time.

- Finally you are provided with your Client ID. Copy and paste it in Flectra.

.. image:: media/google_analytics_client_id.png
    :align: center

- Open your Website Dashboard in Flectra and link your Analytics account. 
  to past your Client ID.

.. image:: media/google_analytics_start.png
    :align: center

- As a last step, authorize Flectra to access Google API.

.. image:: media/google_analytics_login.png
    :align: center
