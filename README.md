# tobias_richter.apt_config

[![Build Status](https://github.com/tobias-richter/ansible-apt-config/workflows/CI/badge.svg)](https://github.com/tobias-richter/ansible-apt-config/actions)

This role configures apt sources, preferences and apt-cacher-ng / proxy for Debian and Ubuntu.

## Requirements

This role requires Ansible 2.7 or higher.

## Role Variables

See [defaults/main.yml](defaults/main.yml) for the documented role variables.
See also the distribution specific [vars](vars).


## Example Playbook

This playbook configures apt together with a proxy server / apt-cacher-ng.

    - hosts: apt_config
	  roles:
	    - role: tobias_richter.apt_config
	      apt_config_http_proxy: http://apt-cacher-ng.main.corp