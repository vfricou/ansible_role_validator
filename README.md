# Ansible Role: validator

![Master Branch Action Status](https://github.com/vfricou/ansible_role_validator/actions/workflows/main.yml/badge.svg?branch=master)

# Disclaimer

I couldn't be responsible with any production issues if you use this role without any prior tests.  
This role is designed for my proper environment and possibly not correspond to your.

The master branch is development branch. Use only release/* branches for production.

# Introduction

This role is designed to perform a basic assertion to exclude unsupported hosts.

# Use cases

This role would be included in playbook before other roles or task to perform preflight check on remote hosts.

# Changelog

To clearest and updated changelog, I encourage you to see pull requests with flags "feature".

# Role variables

Role variables is only used to specify supported OS.  
See [default variables](#default-variables) to get variable structure.

## Default variables

```yaml
---
support:
  Debian: ['10', '11']
  Ubuntu: ['18', '20', '21']
  RedHat: ['8']
  Rocky: ['8']
  AlmaLinux: ['8']

```

# Tests

Initials tests was done through molecule.  
Role fully tested on virtual machines vanilla installed.
