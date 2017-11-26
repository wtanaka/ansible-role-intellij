[![Build Status](https://travis-ci.org/wtanaka/ansible-role-intellij.svg?branch=master)](https://travis-ci.org/wtanaka/ansible-role-intellij)
[![CircleCI](https://circleci.com/gh/wtanaka/ansible-role-intellij.svg?style=svg)](https://circleci.com/gh/wtanaka/ansible-role-intellij)

wtanaka.intellij
================

Installs IntelliJ IDEA

Example Playbook
----------------

    - hosts: servers
      roles:
         - wtanaka.intellij

Install a specific version

    - hosts: servers
      roles:
         - role: wtanaka.intellij
           intellij_version: "2017.1.3"
           intellij_include_jdk: False

The full set of configuration options available are visible in
[defaults/main.yml](defaults/main.yml)

### `intellij_install_dir`

Directory to install IntelliJ IDEA in, like `/opt/intellij`

### `intellij_version`

Version, like `2017.1.3`

### `intellij_include_jdk`

boolean, true to download the package with the JDK, or false to
download the package without the JDK

License
-------

GPLv2

Author Information
------------------

http://wtanaka.com/
