Ansible Role: Traefik
=========

An ansible role to install Traefik as a systemd service.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```
traefik_version: "v3.7.11"
traefik_service_name: "traefik"

traefik_repo_url: "https://github.com/traefik/traefik"

traefik_system_user: "traefik"
traefik_system_group: "traefik"
traefik_bin_dir: "/usr/local/bin"
traefik_log_dir: "/var/log/traefik"
```


Example Playbook
----------------

Install Treafik as a systemd service

    - hosts: servers
      become: true
      roles:
         - { role: w0.traefik, traefik_version: v3.7.10}

License
-------

Apache-2.0
