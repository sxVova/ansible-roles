Letsencrypt role
=========

This role installs nginx and letsencrypt. The role automatic issuing and attaching a certificate and redirect traffic to the desired port

Role Variables
--------------

| Variable                                                                                                                                        | Description                                                                                                                                                                                                                                              |
|-------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `ansible_user`                                                                                                                         | Your Ansible user name.|
| `ansible_ssh_private_key_file`                                                                                                          | Path to ssh private key. |
| `letsencrypt_email`                                                                                                                   | Email for attaching SSL certificate.|

Example Playbook
----------------

    - hosts: letsencrypt
      become: true
      roles:
         - { role: letsencrypt_role }

License
-------

GNU General Public License v3.0

Author Information
------------------

https://www.sxvova.opensource-ukraine.org/
