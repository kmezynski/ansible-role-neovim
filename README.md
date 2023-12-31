[![CI](https://github.com/kmezynski/ansible-role-neovim/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/kmezynski/ansible-role-neovim/actions/workflows/ci.yml)
[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kmezynski/ansible-role-neovim/master.svg)](https://results.pre-commit.ci/latest/github/kmezynski/ansible-role-neovim/master)
[![License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE)
[![Code of Conduct](https://img.shields.io/badge/code%20of%20conduct-Ansible-silver.svg)](.github/CODE_OF_CONDUCT.md)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)

# Ansible Role: Neovim

Installs [Neovim](https://neovim.io) with or without [Packer](https://github.com/wbthomason/packer.nvim)
plugin manager on RHEL or Debian/Ubuntu servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (refer to
[defaults](defaults) and [vars](vars) directories).

```yaml
neovim_git_ref: master
neovim_path: /usr/local
```

These variables control Neovim installation process:

- `neovim_path` - path to Neovim binary (`bin/nvim` is appended automatically).
- `neovim_git_ref` - git reference of [Neovim repository](https://github.com/neovim/neovim)
  to be installed.

```yaml
neovim_packer: false
neovim_packer_config_path: "{{ ansible_user_dir }}/.config/nvim/lua/custom"
```

Above variables configures Packer plugin manager installation:

- `neovim_packer` - enables Packer installation.
- `neovim_packer_config_path` - path to Packer's basic configuration.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  roles:
    - role: kmezynski.neovim
      neovim_git_ref: v0.9.1
      neovim_path: /usr # bin/nvim is appended automatically
      neovim_packer: true
```

## License

This role is distributed under the terms of [MIT](https://opensource.org/license/mit/)
license.

## Author Information

This role was created in 2023 by [Kamil Mężyński](https://github.com/kmezynski).
