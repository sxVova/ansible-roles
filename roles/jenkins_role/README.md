Jenkins role
=========

This role installs pip and works in virtualenv. Role installs java and jenkins, downloads data from gcloud storage and makes backup.

Role Variables
--------------

jenkins-restore.sh - script to restore backup from an archive
jenkins-backup.sh - script to create an archive for future restore
jenkins-backup.yml - playbook to create an archive and upload it to the gcloud storage 

Example Playbook
----------------

    - hosts: jenkins
      roles:
         - { role: jenkins }

License
-------

BSD

Author Information
------------------

https://www.sxvova.opensource-ukraine.org/
