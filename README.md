Ansible Role: gitea
=========

Installs Gitea on Linux machines.

Requirements
------------

Permission to:
  - Install dependency packages
  - Create or modify users/groups
  - Create or modify required directories

Role Variables
--------------
A list of available variables is listed below, along with their default vaules.

    gitea_version: 1.20.1

The version of Gitea to install.

    gitea_user: gitea
    gitea_group: gitea

The user and group that will be created and Gitea will run under.

    gitea_daemon: gitea

The name of the service used to control the Gitea process.

    gitea_home_dir: /home/gitea
    gitea_data_dir: /var/lib/gitea
    gitea_bin_dir: /usr/local/bin
    gitea_config_dir: /etc/gitea

Default folders created for Gitea binaries and data.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: bcook254.gitea
           become: yes

License
-------

MIT / BSD

Author Information
------------------

This role was created by Benjamin Cook.
