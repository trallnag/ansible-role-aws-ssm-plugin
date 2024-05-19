# Ansible Role `trallnag.aws_ssm_plugin` <!-- omit from toc -->

Role that installs the
[Session Manager plugin for the AWS CLI](https://github.com/aws/session-manager-plugin).

Available on
[Ansible Galaxy](https://galaxy.ansible.com/ui/standalone/roles/trallnag/aws_ssm_plugin).

## Table of Contents <!-- omit from toc -->

- [Requirements](#requirements)
- [Role Parameters](#role-parameters)
- [Project Status](#project-status)
- [Contributing](#contributing)
- [Licensing](#licensing)

## Requirements

Some tasks require root privileges. Privilege escalation is performed with
explicit `become: true` statements.

## Role Parameters

See [`meta/argument_specs.yml`](meta/argument_specs.yml).

```yaml
aws_ssm_plugin_version:
  required: false
  type: str
  default: present
  description:
    - Version of the Session Manager plugin for the AWS CLI to install.
    - Use special value `present` to install latest version once.
    - Use special value `latest` to always install latest version.
    - Exact versions like `1.2.553.0` are not supported.
```

## Project Status

Maintained and actively used.

## Contributing

Contributions are welcome. Please refer to [`CONTRIBUTING.md`](CONTRIBUTING).

Consult [`DEVELOPMENT.md`](DEVELOPMENT.md) for guidance regarding development.

Read [`RELEASE.md`](RELEASE.md) for details about the release process.

## Licensing

This work is licensed under the
[Apache License](https://choosealicense.com/licenses/apache-2.0) (Apache-2.0), a
permissive license whose main conditions require preservation of copyright and
license notices. See [`LICENSE`](LICENSE) for the license text.

This work comes with an explicit [`NOTICE`](NOTICE) file containing additional
legal notices and information.
