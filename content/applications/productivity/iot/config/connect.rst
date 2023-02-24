=======================================
Connect an IoT Box to the Odoo database
=======================================

Install the Internet of Things (IoT) App on the Odoo database.

.. image:: connect/connect01.png
   :align: center
   :alt: The Internet of Things (IoT) App on the Odoo database.

Go to the IoT App and click on Connect on the IoT Boxes page.

.. image:: connect/connect-iot.png
   :align: center
   :alt: Connecting an IoT box to the Odoo database.

Follow the steps to connect the IoT Box.

.. image:: connect/connect03.png
   :align: center
   :alt: Connection steps for a wired connection or WiFi connection.

Ethernet Connection
===================

#. Connect to the IoT Box all the devices that have to be connected with
   cables (ethernet, usb devices, etc.).

#. Power on the IoT Box.

#. Read the Pairing Code from a screen or a receipt printer connected to the IoT Box.

   .. image:: connect/connect04.png
       :align: center
       :alt: Pairing code for a wired connection.

..
   _Image needs to be updated.

#. Input the Pairing Code on the IoT module of the database and click on the Pair button.

.. note::
   Recent changes in modern web browsers forced us to modify the connection wizard. If the screen is
   different from the screenshots, make sure that the ``iot_pairing`` module is installed.

..
   _This module doesn't exist any longer.

WiFi Connection
===============

#. Power on the IoT Box

#. Copy the token from the WiFi connection section in IoT module of the Odoo database.

   .. image:: connect/connect05.png
      :align: center
      :alt: Pairing Token for a WiFi connection.

#. Connect to the IoT Box WiFi Network (make sure there is no ethernet cable plugged in the
   computer).

   .. image:: connect/connect06.png
      :align: center
      :alt: WiFi networks available on the computer.

..
   _Image needs to be updated.

#. Upon connecting to the IoT WiFi a browser will automatically redirect to the IoT Box Homepage (if
   it doesn't work, connect to the IP address of the box). The default address of the IoT box is
   `localhost:8069 <http://localhost:8069/>`. Give a name to the IoT Box (not required), paste the
   previously copied token, and then click on next.

   .. image:: connect/connect07.png
      :align: center
      :alt: A connection has been made with the IoT box and Odoo database.

   .. tip::
      If the configuration is on Runbot, do not forget to add the -all or -base in the
      token (e.g. this token
      **http://375228-saas-11-5-iot-f3f920.runbot16.odoo.com\|4957098401**
      should become
      **http://375228-saas-11-5-iot-f3f920-all.runbot16.odoo.com\|4957098401**).

..
  _Confirm the web address prior to entering the token.

#. Choose the WiFi network that the IoT box will connect with (enter the password if there is one)
   and click on Submit. Wait a few seconds before being redirected to the database. The computer may
   need to be manually connected back to WiFi.

   .. image:: connect/connect08.png
      :align: center
      :alt: Configuring the WiFi for the IoT box.

The IoT box should appear in the IoT module of the Odoo database.

.. image:: connect/connect09.png
   :align: center
   :alt: The IoT box has been successfully configured on the Odoo database.

IoT Box Schema
==============

.. image:: connect/connect10.png
      :align: center
      :alt: Odoo IoT box schema with labels.
