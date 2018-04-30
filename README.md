Nextcloud
=========

A role to install Nextcloud on RHEL 7 & CentOS 7

Requirements
------------

None

Role Variables
--------------

| name | default | comments |
|------|---------|----------|
| nextcloud_package_url | `https://download.nextcloud.com/server/releases/nextcloud-13.0.2.tar.bz2` | URL to download the nextcloud package from |
| nextcloud_package_destination | `"{{ ansible_env.HOME }}"` | This is a temporary location to download the package to. Generally doesn't need to be tweaked. |
| nextcloud_use_firewalld | yes | Whether or not `firewalld` is in use on the remote |

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - shouptech.nextcloud

License
-------

BSD

Author Information
------------------

Mike Shoup <mike@shouptech.com>
