Install SSH CA
=========

A very simple role to install an SSH-Sentinel CA onto a server

Requirements
------------

No specific ansible requirements but you will need a running SSH-Sentinel CA install

Role Variables
--------------

You will need to set 2 variables:

- `auth_url` - This is the URL of your running sentinel server
- `key_file` - The filename of the CA to be stored on the target server


Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: neo1908.install_ssh_ca, auth_url: "https://auth.domain.com", key_file: "/etc/ssh/ca.pub" }

License
-------

GPLv3
