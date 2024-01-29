# Ansible collection skeleton

|||
|---|---|
|master|![master branch CI](https://github.com/mafalb/ansible_collection_skeleton/actions/workflows/CI.yml/badge.svg)|
|dev|![dev branch CI](https://github.com/mafalb/ansible_collection_skeleton/actions/workflows/CI.yml/badge.svg?branch=dev)|

Use it with ansible-galaxy when you use init.
Jinja templates are processed by ansible-galaxy and have precedence over the non template counterparts. This README is one example of that.

`README.md` -> this file
`README.md.j2` -> becomes the README.md5 in the newly initialized collection.

You can find a similar role skeleton at
https://github.com/mafalb/ansible_role_skeleton.git

>>>>>>> dev

## Basic Usage

```shell
[ansible_collections] $ git clone https://github.com/mafalb/ansible_collection_skeleton /tmp/ansible_collection_skeleton
```

```shell
[ansible_collections] $ ansible-galaxy collection init --collection-skeleton /tmp/ansible_collection_skeleton local.mycollection
```

## CI

There is a related repository which is partly derived from this repository and is located at
https://github.com/mafalb/ansible-test-collections.git

At least one of these collections in that repo is periodically initialized from this skeleton by CI.

```shell
[ansible_collections] $ ansible-galaxy collection install git+https://github.com/mafalb/ansible-test-collections.git,dev -p collections
```

## License

Copyright (c) Markus Falb <markus.falb@mafalb.at>

GPL-3.0-or-later
