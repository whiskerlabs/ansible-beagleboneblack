# armsible-bbb

An Ansible role for provisioning BeagleBone Black devices.

This role installs a fix for a known issue that prevents `apt-get
install` from working on revision C of the BBB [1] and provides hooks
for installing custom device tree overlays and setting uEnv.txt
options.

[1] https://groups.google.com/forum/#!topic/beagleboard/LPjCn4LEY2IAn

## Installation

To install from Ansible Galaxy:

    $ ansible-galaxy install armsible.bbb

Or alternatively, add the path to a local copy of this repository to
`roles_path` within your project's `ansible.cfg` file:

    roles_path = /path/to/role_dir

where `/path/to/role_dir` is a parent directory of
`armsible-bbb`.

Consult
[Ansible documentation](http://docs.ansible.com/intro_configuration.html)
for more info on how to configure `roles_path` in an Ansible
configuration file.

## Requirements

`armsible-bbb` has no role dependencies and should work with BBBs
running any version of Linux.

## Role Variables

See documentation in `defaults/main.yml`.

## License

Copyright 2015 Whisker Labs

Licensed under the MIT License. See `LICENSE` for details.