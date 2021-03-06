
===============
fritzconnection
===============


.. image::
    https://img.shields.io/pypi/pyversions/fritzconnection.svg
    :alt: Python versions
    :target: https://pypi.org/project/fritzconnection/

.. image::
    https://img.shields.io/pypi/l/fritzconnection.svg
    :target: https://pypi.org/project/fritzconnection/


Python-Tool to communicate with the AVM FritzBox.
Uses the TR-064 protocol over UPnP.

Installation:
-------------

    pip install fritzconnection


Quickstart:
-----------

Using fritzconnection is as easy as: ::

    from fritzconnection import FritzConnection

    fc = FritzConnection(address='192.168.178.1')
    fc.reconnect()  # get a new external ip from the provider
    print(fc)  # print router model informations

In general FritzConnection can execute every action provided by the (model-specific) API. For i.e. this can be WLAN settings, internet connection and device status informations, home automation services and much more. The package comes with a library providing some modules as examples how to implement applications on top of FritzConnection.


Documentation
-------------

The full documentation and release notes are at https://fritzconnection.readthedocs.org
