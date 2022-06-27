ansible_hardening
=================

This is the AnySURE role ansible_hardening.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

| Variable | default | options | description |
|----------|---------|---------|-------------|
| resolv_nameservers| a base list | | A list of up to 3 nameserver IP addresses 
| resolv_domain | our internal domain | "" | string |
| resolv_search | our internal domain | list | List of up to 6 domains to search for host-name lookup  | 
| resolv_sortlist | [] | list | List of IP-address and netmask pairs to sort addresses returned by gethostbyname. |
| resolv_options | [] | list | List of options to modify certain internal resolver variables. |

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - ansible_hardening

License
-------

Apache 2.0

Author Information
------------------

Ronny Roethof <ronny.roethof@anylinq.com>
