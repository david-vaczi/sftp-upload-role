# SFTP Upload role

## Description

The role provides a wrapper for AWX to upload data to the target SFTP server.

## Prerequisites

* Ansible version >= 2.7
* community.general collection
* zipfile package on localhost (or your Execution Enviroment when using AWX)
* some custom credentials to be detailed later

### Custom Credentials

TBD

## Usage

TBD

### Variables

TBD

### Playbook example

```
- name: Example playbook
  hosts: all
  tasks:
    - include_role:
        name: sftp-upload-role
        vars:
        phase: "prepare"

    <Your other tasks or roles>

    - include_role:
        name: sftp-upload-role
        vars:
        phase: "upload"
```

## License

GNU GPLv3

## Author
David Vaczi