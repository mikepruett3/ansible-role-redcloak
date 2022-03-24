Ansible Role: Red Cloak ATP
=========

Ansible role to install Red Cloak ATP on Linux Servers.

Requirements
------------

The role does not require anything to run on RHEL or Debian and its derivatives.

Role Variables
--------------

Available variables are listed below, along with default values (see ```defaults/main.yml```):

``` yaml
password_authentication: "no"

```

Additional (**Optional**) variable is **sshd_config**. This is used to restrict what groups of users can SSH into the server, via the **AllowGroups** configuration in the sshd_config file. This group can be either local or some other external group (like *LDAP/AD*). If this variable is not defined, then the default SSH config will allow any valid user to login via SSH.

Role variables can be stored with the hosts.yaml file, or in the main variables file.

Dependencies
------------

None.

Example Playbook
----------------

``` yaml
    - hosts: servers
      roles:
         - role: mikepruett3.redcloak
```

License
-------

MIT

Author Information
------------------

Role created by [mikepruett3](https://github.com/mikepruett3) on [Github.com](https://github.com/mikepruett3/ansible-role-redcloak)
