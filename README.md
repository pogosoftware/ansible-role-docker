Docker
=========

This role will install and configure docker.

Role Variables
--------------

* `docker.install_docker_compose` - Determinate if install docker compose or not
* `docker.docker_compose_version` - docker compose version
* `docker.users` - Users that will be added to the docker group

Example Playbook
----------------

```yaml
- hosts: localhost
  become: yes
  roles:
    - pogosoftware.docker
  vars:
    docker:
      install_docker_compose: yes
      docker_compose_version: '1.24.1'
      users:
        - vagrant
```

  
