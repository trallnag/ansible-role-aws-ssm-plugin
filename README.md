[![status](https://img.shields.io/badge/status-active-brightgreen)](#project-status)
[![release](https://img.shields.io/github/v/release/trallnag/ansible-role-aws-ssm-plugin)](https://github.com/trallnag/ansible-role-aws-ssm-plugin/releases)
[![ci](https://img.shields.io/github/actions/workflow/status/trallnag/ansible-role-aws-ssm-plugin/ci.yaml?label=ci)](https://github.com/trallnag/ansible-role-aws-ssm-plugin/actions/workflows/ci.yaml)
[![release](https://img.shields.io/github/actions/workflow/status/trallnag/ansible-role-aws-ssm-plugin/release.yaml?label=release)](https://github.com/trallnag/ansible-role-aws-ssm-plugin/actions/workflows/release.yaml)

# Ansible Role `trallnag.aws_ssm_plugin`

Role that installs the
[Session Manager plugin for the AWS CLI](https://github.com/aws/session-manager-plugin).

Available on
[Ansible Galaxy](https://galaxy.ansible.com/ui/standalone/roles/trallnag/aws_ssm_plugin).

## Requirements

Some tasks require root privileges. Privilege escalation is performed with
explicit `become: true` statements.

## Role parameters

See [`meta/argument_specs.yml`](./meta/argument_specs.yml).

```yaml
aws_ssm_plugin__version:
  required: false
  type: str
  default: present
  description:
    - Version of the Session Manager plugin for the AWS CLI to install.
    - Use special value `present` to install latest version once.
    - Use special value `latest` to always install latest version.
    - Exact versions like `1.2.553.0` are not supported.
```

## Project status

The project is maintained by me, [Tim](https://github.com/trallnag), and I am
interested in keeping it alive as I am actively using it.

## Versioning

The project follows [Semantic Versioning](https://semver.org/).

## Contributing

Contributions are welcome. Please refer to [`CONTRIBUTE.md`](./CONTRIBUTE.md).

## Licensing

This work is licensed under the
[ISC license](https://en.wikipedia.org/wiki/ISC_license). See
[`LICENSE`](./LICENSE) for the license text.

## Template

This project is based on the following
[Copier](https://copier.readthedocs.io/en/stable/) template:
<https://github.com/trallnag/copier-template-ansible-role>.
