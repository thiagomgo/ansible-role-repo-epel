# **Ansible Role: Repo Epel**

[![Build Status](https://travis-ci.org/thiagomgo/ansible-role-repo-epel.svg?branch=master)](https://travis-ci.org/thiagomgo/ansible-role-repo-epel) [![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-repo--epel-blue.svg)](https://galaxy.ansible.com/thiagomgo/repo-epel/)

A simple ansible role to install EPEL repository.

## Requirements

This role only requires Ansible version 1.9+.

## Role Variables

Here is a list of all the default variables for this role, which are also available in `defaults/main.yml`.

```yaml
---

epel_repo_url: "https://dl.fedoraproject.org/pub/epel/epel-release-latest-{{ ansible_distribution_major_version }}.noarch.rpm"
epel_repo_gpg_key_url: "/etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-{{ ansible_distribution_major_version }}"

```

## Dependencies

None

## Example Playbook

```yaml
---

- hosts: all

  roles:
    - ansible-role-repo-epel

```

## License

MIT / BSD

## Author Information

Thiago Gomes
- thiago.mgomes [at] gmail.com
