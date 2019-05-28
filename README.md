ansible-nginx-slac
=================

Demonstrate testing with Molecule, Vagrant, Travis CI and Goss

Role Variables
--------------

    nginx_heading: Welcome to nginx!

Define `gost_test_directory` to copy Goss tests there.

Example Playbook
----------------

    - hosts: localhost
      become: true
      roles:
        - ansible-nginx-slac
        - base_goss
      vars:
        nginx_heading: Hello SLAC!
        goss_test_directory: /etc/goss.d

License
-------

GPLv3
