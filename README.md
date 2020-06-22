ddclient
========

[![Build Status](https://travis-ci.org/kurtabersold/ddclient.svg?branch=master)](https://travis-ci.org/kurtabersold/ddclient)

This role installs and configures DDclient. 'DDclient is a Perl client used to update dynamic DNS entries for accounts on Dynamic DNS Network Service Provider.'

Requirements
------------

This role requires Ansible 1.4 or higher, and platform requirements are listed in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows:

    ddclient_ssl: "no"
    ddclient_protocol: "namecheap"
    ddclient_use: "web, web=checkip.dyndns.org/"
    ddclient_server: "dynamicdns.park-your-domain.com"
    ddclient_login: "mydomain.com"
    ddclient_password: "'MY_PASSWORD'"
    ddclient_subdomain: "mysubdomain"                    # For example mysubdomain.example.com

Dependencies
------------

None


TODO
------------

Make some options optional. For example if we do not want to include the 'use' line at all, or we do not want to use a subdomain.

Add in defaults for well known domain registrars.

License
-------

MIT

Author Information
------------------

Original: Jonathan Rowlands

This is forked from Jonathan's code.

