Ubuntu-Ghost Installation
=========================

This role will grab the latest release of ghost, install it on ubuntu 14.04(trusty), provide it with basic configuration, and bring Ghost online .

Requirements
------------

  * None

Role Variables
--------------

  * ghost_path: The full path where ghost is deployed
  * ghost_port: What port ghost will listen on
  * ghost_ver: Currently set to latest, need to find further reference on their dl page for version drop in
  * ghost_url: URL for ghost, IP works well for dev. Role will use the targets IP as url unless adjusted.
  * site_type: production, development callable NODE_ENV's in config.js

Dependencies
------------

  * None.

Example Playbook
-------------------------

    - hosts: servers
      roles:
         - {{ role: ansible-ghost }}


License
-------

BSD

Author Information
------------------

No comment.
