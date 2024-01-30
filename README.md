# Skeletons

|||
|---|---|
|master|![master branch CI](https://github.com/mafalb/skeletons/actions/workflows/CI.yml/badge.svg)|
|dev|![dev branch CI](https://github.com/mafalb/skeletons/actions/workflows/CI.yml/badge.svg?branch=dev)|


## Ansible collection skeleton

Use it with ansible-galaxy when you use init.

You can find a similar role skeleton at
https://github.com/mafalb/ansible_role_skeleton.git


## Basic Usage

```shell
[ansible_collections] $ git clone https://github.com/mafalb/skeletons /tmp/skeletons
```

```shell
[ansible_collections] $ ansible-galaxy collection init --collection-skeleton /tmp/skeletons/ansible-collection-skeleton local.mycollection
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
