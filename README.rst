============
Starbucks-py
============

Unofficial Starbucks API.

This API is written in Python.

*Only supports for Starbucks Korea.*


Installation
------------

You can install Starbucks with ``pip``

::

    $ pip install starbucks


Features
--------

1. Login
~~~~~~~~

You can login to Starbucks like:

::

    from starbucks import Starbucks
    
    starbucks = Starbucks()
    starbucks.login('username', 'password')
    


2. Get My Card Information
~~~~~~~~~~~~~~~~~~~~~~~~~~

You can get your card information like:

::

    # You should know the registration number of your card.
    # It is in the source code of Starbucks web page.
    card = starbucks.get_card_info('0000000')
    


3. Logout
~~~~~~~~~

If you want to logout, just:

::

    starbucks.logout()
    


Known Issues
------------

- After the first login, I can't get the card information. But after logout, and login again, then finally I can get the card information.
- Should I have to check if I logged in successfully like this?


To Do
-----

- Cards list
- Card usage histories
- and so on.
