jenkins
===============

This roles installs the Jenkins LTS server, running in a Docker container on the target machine.

Requirements
------------

This role requires Ansible 1.4 or higher

Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows with defaults shown:

```yaml
# Jenkins Docker image name at DockerHub
jenkins_docker_image: openedge/jenkins

# Path on target machine to mount as Jenkins' home
jenkins_home_path: /jenkins
```

Examples
--------

- hosts: somehost
  sudo: yes
  remote_user: someuser

  roles:
    - jenkins

Dependencies
------------

docker
pip

License and Copyright
-----------------------
Copyright 2015 VMware, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

Author Information
---------------------
This role was created in 2015 by [Eric Smalling / VMware](http://www.vmware.com/).

