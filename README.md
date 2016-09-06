ansible-role-hosts-int
======================

Populate /etc/hosts with IP addresses for an internal cluster network, including IB addresses.

Requirements
------------

The hosts in the ansible hosts file must have a variable int_ip_addr
specifying the IP address to use, and ib_ip_addr for the Infiniband
address.

Role Variables
--------------

intDomain: The internal subdomainname
siteDomain: The external site domain name
hosts_int_file_to_populate: /etc/hosts

The generated hosts file will have entries with the domain intDomain.siteDomain.

Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: ansible-role-hosts-int }

License
-------

GPLv3

Author Information
------------------

https://github.com/jabl
