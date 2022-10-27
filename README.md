targetcli-modules
=================

This is a fork of [OndrejHome/ansible.targetcli-modules](https://github.com/OndrejHome/ansible.targetcli-modules) that will hopefully work again with `ansible-galaxy`.

Modules for interacting with targetcli command line utility.

Requirements
------------

*targetcli* utility is expected to be installed on machine.

Role Variables
--------------

None. This role is intended to be included as dependency.

Provided Modules
----------------
*targetcli_backstore* - create/delete backstore objects ('/backstore')

*targetcli_iscsi* - create/delete iscsi object ('/iscsi')

*targetcli_iscsi_lun* - add/remove luns to/from iscsi object ('/iscsi/.../tpg1/luns')

*targetcli_iscsi_acl* - add/remove acls to/from iscsi object ('/iscsi/.../tpg1/acls')

*targetcli_iscsi_portal* - add/remove portals to/from iscsi object ('/iscsi/.../tpg1/portals')

*library/targetcli_iscsi_acl_mapped_lun* - add/remove intividual LUNs to/from ACLs within target ('/iscsi/.../tpg1/acls/.../')

Example Playbook
----------------

Example playbook for including modules in your playbook

    - hosts: servers
      roles:
         - { role: 'yeoldegrove.targetcli_modules' }

License
-------

GPLv3

Kudos to original Author
------------------

To get in touch with the original author you can use email ondrej-xa2iel8u@famera.cz.

