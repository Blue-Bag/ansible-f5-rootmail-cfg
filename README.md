Root Mail Configure
===================
[![Build Status](https://travis-ci.org/Blue-Bag/ansible-role-first5rootmail.svg?branch=master)](https://travis-ci.org/Blue-Bag/ansible-role-first5rootmail)

Originally part of our Exim 4 Role.
This has been spun off to a configure role to keep Exim4 tight.

This sets the default mail address for the server.

Requirements
------------

Although not required it is designed to work after the Exim4 role

Role Variables
--------------

The only vars needed are:
 the server from email (rootmail_server_from_email) e.g.  ansible_hostname@example.com
 the server domainname:  ((rootmail_server_mailname))  e.g. example.com

Dependencies
------------

None (but works with Exim4)

Example Playbook
----------------



    - hosts: servers
      roles:
         - { role: ansible-role-first5rootmail, tags; "mail", "configuration" }

License
-------

BSD

Author Information
------------------

George Boobyer (Blue-Bag)
