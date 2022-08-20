Ansible Role: Domain Tools
=========

Ansible role that provides tools for Domain Management on Linux Servers.

Requirements
------------

The role does not require anything to run on Ubuntu, Debian or RHEL and its derivatives.

Role Variables
--------------

Available variables are listed below, along with default values (see ```defaults/main.yml```):

``` yaml
clientIP: "1.1.1.1"

#NameCheap API Settings
nc_url: "https://api.sandbox.namecheap.com/xml.response"
nc_username: "api"
nc_key: "api-key"
```

```clientIP:``` **(Required)** IP Address to use when calling the API.

```nc_url:``` **(Required)** NameCheap API URL.

```nc_username:``` **(Required)** Username to use with NameCheap API URL.

```nc_key:``` **(Required)** API Key to use with NameCheap API URL.

Role variables can be stored with the ```hosts.yaml``` file, or in the main variables file.

Dependencies
------------

None.

Example Playbook
----------------

``` yaml
    - hosts: servers
      roles:
         - role: mikepruett3.domain-tools
```

License
-------

MIT

Author Information
------------------

Role created by [mikepruett3](https://github.com/mikepruett3) on [Github.com](https://github.com/mikepruett3/ansible-role-domain-tools)
