# docker

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![GitHub release](https://img.shields.io/github/release/codeyourinfra/docker.svg)](https://github.com/codeyourinfra/docker/releases/latest) [![Build status](https://travis-ci.org/codeyourinfra/docker.svg?branch=master)](https://travis-ci.org/codeyourinfra/docker) [![Ansible Role](https://img.shields.io/ansible/role/29242.svg)](https://galaxy.ansible.com/codeyourinfra/docker) [![Ansible Role downloads](https://img.shields.io/ansible/role/d/29242.svg)](https://galaxy.ansible.com/codeyourinfra/docker)

Ansible role to install [Docker](https://www.docker.com).

## Example Playbook

```yml
---
- hosts: servers
  roles:
    - codeyourinfra.docker
```

The role requires the *ansible_distribution_release* variable, obtained through the [gathering facts phase](https://docs.ansible.com/ansible/latest/user_guide/playbooks_variables.html#information-discovered-from-systems-facts). So please don't turn off facts.

## Build process

The build process is performed in [Travis CI](https://travis-ci.org/codeyourinfra/docker). During the build, the role is tested by using [Molecule](https://molecule.readthedocs.io).

If the build is succeeded, dependent roles may have also its builds triggered, thanks to the [travis-dependent-builds project](https://github.com/stephanmg/travis-dependent-builds). One example is the [Codeyourinfra docker-compose Ansible role](https://galaxy.ansible.com/codeyourinfra/docker_compose).

## Test yourself

First of all, create your [Python virtual environment](https://docs.python.org/3/tutorial/venv.html) and activate it:

`python -m venv env && source env/bin/activate`

After that, install all requirements:

`pip install wheel && pip install -r requirements.txt`

Finally, execute the test:

`molecule test`

## Author Information

[@gustavomcarmo](https://github.com/gustavomcarmo) is a contributor of [Codeyourinfra](https://github.com/codeyourinfra). Get on board too! :)
