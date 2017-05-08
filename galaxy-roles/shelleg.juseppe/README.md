Ansible Role Juseppe
====================

Your very own jenkins update site [ Docker based ] running on localhost:9090

Requirements
------------

Docker daemon - recommend using [ansible-role-simple-docler-deamon role](https://galaxy.ansible.com/shelleg/simple-docker-daemon/)

Role Variables
--------------

* `juseppe_container_hostname: juseppe`
* `juseppe_container_name: lanwen/juseppe`
* `juseppe_container_tag: 1.0.0`
* `juseppe_container_port: 8080`
* `juseppe_host_port: 9090`
* `juseppe_docker_host_ip: localhost`

* `juseppe_cert_dir: /var/lib/juseppe`
* `juseppe_plugin_cache_dir: /var/cache/juseppe`

```python
juseppe_plugins:
  - { name: "credentials-binding",  version: "1.10" }
  ... 
```  
Dependencies
------------

A Docker daemon running on the host.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: juesppe

License
-------

MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
