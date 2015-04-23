Root Mail Configure
===================

Originally part of our Exim 4 Role.
This has been spun off to a configure role to keep Exim4 tight.

This sets the default mail address for the server.

Requirements
------------

Although not required it is designed to work after the Exim4 role

Role Variables
--------------

The only var beeded is the server from email (rootmail_server_from_email)

Dependencies
------------

None (but works with Exim4)

Example Playbook
----------------



    - hosts: servers
      roles:
         - { role: ansible-rootmail-cgf, tags; "mail", "configuration" }

License
-------

BSD

Author Information
------------------

George Boobyer (Blue-Bag)
