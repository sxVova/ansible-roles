Docker role
=========

This role installs docker and docker-compose.


Example Playbook
----------------

    - hosts: all
      become: true
      roles:
         - { role: docker_role }

License
-------

BSD

Author Information
------------------

https://www.sxvova.opensource-ukraine.org/
