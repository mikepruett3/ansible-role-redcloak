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
software_url: "http://www.example.org"
package_name: "redcloak-1.2.15.0_x86_64.rpm"
```

```software_url``` **(Required)** The URL that hosts the Installer package. This should be either **http** or **https**.

```package_name``` **(Required)** The Installer package name.

Role variables can be stored with the ```hosts.yaml``` file, or in the main variables file.

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
