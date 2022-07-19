Role Name
=========

Install bitlbee with a simple configuration

Requirements
------------

Nothing special.

Role Variables
--------------

Required Variables:
 - vault_bitlbee_auth_password
 - vault_bitlbee_op_password

Dependencies
------------

This role expects a pre-existing certificate and key (see defaults/main.yml). These will be provisioned with the `ansible-role-acme-cert`, if you've already run that or specify that role first.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: server
      vars:
        vault_bitlbee_auth_password: ChangeMe
        vault_bitlbee_op_password: ChangeMe2
      roles:
         - ansible-role-acme-cert
         - ansible-role-bitlbee

License
-------

MIT

Author Information
------------------

Mike Oliver (mike@mklvr.io)
