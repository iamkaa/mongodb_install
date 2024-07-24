# Mongodb Install

Ansible role just for installing MongoDB.

## vars:
* mongo_major_release: - major release, defailt is '7.0'.
* mongo_minor_release: - rapid release, default is '*' meaning latest version.

## How to use

Role required root privileges, so set `become = True` whatever you want.

Example playbook:

	---
	- name: Mongodb config
          hosts: all

          roles:
          - mongodb_config


## Compatibility 

MongoDB versions:
- 7.0.12

Linux distributions:
- Rocky 9.0
- Ubuntu 22.04

## How to test

Default test scenario runs role with default vars on distros:

- Rocky 9.0
- Ubuntu 22.04

Run test: `molecule test`

## Author

iamkaa
