Role Name
=========

This role installs nginx and letsencrypt. The role automatic issuing and attaching a certificate and redirect traffic to the desired port

Role Variables
--------------

nginx.conf.j2, nginx-le.j2, nginx-http.j2 - сonfiguration files necessary for automatic issuing and attaching a certificate and redirect traffic to the desired port.


Example Playbook
----------------

    - hosts: letsencrypt
      roles:
         - { role: letsencrypt }

License
-------

BSD

Author Information
------------------

https://www.sxvova.opensource-ukraine.org/
