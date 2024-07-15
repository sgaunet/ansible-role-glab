
# Ansible Role: glab

[![CI](https://github.com/sgaunet/ansible-role-glab/workflows/CI/badge.svg)](https://github.com/sgaunet/ansible-role-glab/actions?query=workflow%3ACI)

An Ansible Role that installs glab on Linux.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    glab_bin_path: "/usr/local/bin/glab"
    glab_tmp_directory: "{{ lookup('env', 'TMPDIR') | default('/tmp', true) }}"
    glab_os: "Linux"
    glab_arch: "x86_64"

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  roles:
    - sgaunet.glab
```

## License

MIT
