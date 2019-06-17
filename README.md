# ansible-role-jenkins

This roles installs the Jenkins LTS server, running in a Docker container on
the target machine.

## Requirements

This role requires Ansible 1.4 or higher.

## Dependencies

- docker
- pip

## Role Variables

The variables that can be passed to this role and a brief description about
them are as follows with defaults shown:

```yaml
# Jenkins Docker image name at DockerHub
jenkins_docker_image: openedge/jenkins

# Path on target machine to mount as Jenkins' home
jenkins_home_path: /jenkins
```

## Examples

```yaml
- hosts: somehost
  sudo: yes
  remote_user: someuser

  roles:
    - jenkins
```

License and Copyright
-----------------------
Copyright 2015 VMware, Inc.

This code is Dual Licensed Apache-2.0 or GPLv3

Author Information
---------------------
This role was created in 2015 by [Eric Smalling / VMware](http://www.vmware.com/).

