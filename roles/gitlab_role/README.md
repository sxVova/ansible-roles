GitLab role
=========

This role installs pip and works in virtualenv. The role installs gitlab, gives an ssl certificate, downloads data from gcloud storage and makes backup.

Role Variables
----------------

| Variable                                                                                                                                        | Description                                                                                                                                                                                                                                              |
|-------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `ansible_user`                                                                                                                         | Your Ansible user name.|
| `ansible_ssh_private_key_file`                                                                                                          | Path to ssh private key. |
| `gitlab_external_url`                                                                                                                 | The link that is used to attach the SSL certificate. |
| `gcloud_storage_key`                                                                                                                   | Gcloud IAM user public key(encrypted)|
| `gcloud_storage_secret_key`                                                                                                           | Gcloud IAM user private key(encrypted) |
| `gcloud_storage_name`                                                                                                                 | Name of Gcloud storage  |
| `gcloud_bucket_name`                                                                                                                   | Name of Gcloud bucket in storage |
| `gcloud_tar_name`                                                                                                                     | Backup archive name |

Example Playbook
----------------

    - hosts: gitlab
      become: true
      roles:
         - { role: gitlab_role }

License
-------

GNU General Public License v3.0

Author Information
------------------

https://www.sxvova.opensource-ukraine.org/
