Jenkins K8s role
=========

This role installs pip, tar, google cloud sdk, kubectl, flake8, nodejs, eslint.  
This role copy service account key file and linter for Java code.

Role Variables
--------------

| Variable                      | Description                                        |
|-------------------------------|----------------------------------------------------|
| `ansible_user`                | Your Ansible user name.                            |
| `ansible_ssh_private_key_file`| Path to ssh private key.                           |


Example Playbook
----------------

    - hosts: jenkins
      become: true
      roles:
         - { role: jenkins_k8s_role }

License
-------

GNU General Public License v3.0

Author Information
------------------

https://www.sxvova.opensource-ukraine.org/
