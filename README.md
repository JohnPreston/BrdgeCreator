Bridge Creator
=========

Creates a bridge on an interface if it doesnt exist already.

Requirements
------------

CentOS / RHEL 6+

Role Variables
--------------

bridge_number : ID for the bridge (brX)
iface_name: Name of the NIC it will be bound to (using the actual network configuration)

Dependencies
------------

[]

Example Playbook
----------------

- hosts: virthost
  roles:
  - BridgeCreator
  vars:
  - iface_name: eth1.200
  - bridge_number: 200


License
-------

GPLv3

Author Information
------------------

John Preston [John Mille]

