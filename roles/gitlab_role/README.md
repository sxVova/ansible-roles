Role Name
=========

This role installs pip and works in virtualenv. The role installs gitlab, gives an ssl certificate, downloads data from gcloud storage and makes backup.

Role Variables
--------------

The gitlab.rb.j2 file contains the necessary configuration for gitlab to work properly.


Example Playbook
----------------

    - hosts: gitlab
      roles:
         - { role: gitlab }

License
-------

BSD

Author Information
------------------

https://www.sxvova.opensource-ukraine.org/
