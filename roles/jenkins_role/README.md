Jenkins role
=========

This role installs pip and works in virtualenv. Role installs java and jenkins, downloads data from gcloud storage and makes backup.

Role Variables
----------------

| Variable                      | Description                                        |
|-------------------------------|----------------------------------------------------|
| `ansible_user`                | Your Ansible user name.                            |
| `ansible_ssh_private_key_file`| Path to ssh private key.                           |
| `gcloud_storage_key `         | Gcloud IAM user public key(encrypted).             |
| `gcloud_storage_secret_key `  | Gcloud IAM user private key(encrypted).            |
| `gcloud_storage_name `        | Name of Gcloud storage.                            |
| `gcloud_bucket_name`          | Name of Gcloud bucket in storage.                  |
| `gcloud_tar_name`             | Backup archive name.                               |

Example Playbook
----------------

    - hosts: jenkins
      become: true
      roles:
         - { role: jenkins_role }

License
-------

GNU General Public License v3.0

Author Information
------------------

https://www.sxvova.opensource-ukraine.org/
