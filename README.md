# Ansible Role: ansible-apps_victoriametrics

## Description

[![Build Status](https://travis-ci.com/lotusnoir/ansible-apps_victoriametrics.svg?branch=master?style=flat)](https://travis-ci.com/lotusnoir/ansible-apps_victoriametrics)
[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen?style=flat)](https://opensource.org/licenses/Apache-2.0)
[![Ansible Role](https://img.shields.io/badge/galaxy-apps_victoriametrics-purple?style=flat)](https://galaxy.ansible.com/lotusnoir/apps_victoriametrics)
![GitHub repo size](https://img.shields.io/github/repo-size/lotusnoir/ansible-apps_victoriametrics?color=orange&style=flat)
![Ansible Quality Score](https://img.shields.io/ansible/quality/52300)
[![downloads](https://img.shields.io/ansible/role/d/52300)](https://galaxy.ansible.com/lotusnoir/apps_victoriametrics)
[![Version](https://img.shields.io/github/release/lotusnoir/ansible-apps_victoriametrics.svg)](https://github.com/lotusnoir/ansible-apps_victoriametrics/releases/)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_victoriametrics&metric=alert_status)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_victoriametrics)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_victoriametrics&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_victoriametrics)
[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_victoriametrics&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_victoriametrics)
[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_victoriametrics&metric=security_rating)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_victoriametrics)

Deploy [victoriametrics](https://victoriametrics.com/) monitoring system.

## Role variables

| Name                      | Default Value | Description                        |
| ------------------------- | ------------- | -----------------------------------|
| `victoriametrics_version` | 0.3.2         | victoriametrics version |

## Examples

	---
	- hosts: apps_victoriametrics
	  become: yes
	  become_method: sudo
	  gather_facts: yes
	  roles:
	    - role: ansible-apps_victoriametrics
	  environment: 
	    http_proxy: "{{ http_proxy }}"
	    https_proxy: "{{ https_proxy }}"
	    no_proxy: "{{ no_proxy }}

## License

This project is licensed under Apache License. See [LICENSE](/LICENSE) for more details.
