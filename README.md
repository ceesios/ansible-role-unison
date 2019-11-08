Role Name
=========

This role installs and configures Unison.

Requirements
------------

-

Role Variables
--------------

|Name|Type|Description|Default|Required|
|----|----|-----------|-------|-------|
`unison.state`|string|`Is this the master or slave`|``|`yes`|
`unison.user`|string|`user that should run the jobs`|`root` |`no`|
`unison.homedir`|string|`homedir of the user`|`/root`|`no`|
`unison.slave_ip`|string|`IP of slave`|``|`yes`|
`unison.slave_inventory_name`|string|`Inventory name of slave`|``|`yes`|
`unison.job`|string|`Details for each syncjob`|``|`yes`|
`job.{item}.name`|string|`Syncjob name`|``|`yes`|
`job.{item}.dir`|string|`Syncjob dir`|``|`yes`|
`job.{item}.ignoredpaths.{item}`|string|`Syncjob ignoredpaths`|``|`no`|

Dependencies
------------

-

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - ceesios.unison

License
-------

GNU General Public License v3.0 

Author Information
------------------

- [Cees Moerkerken](https://virtu-on.nl)