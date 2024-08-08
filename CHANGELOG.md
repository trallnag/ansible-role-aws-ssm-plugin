# Changelog

All notable changes to this project are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0),
and adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0).

## Unreleased

### Changed

- Changed executable for shell tasks from `/usr/bin/bash` to `/bin/bash`.
- Switched permissions of temporary artifacts from `u=rw,g=r,o=r` to
  `u=rw,g=,o=`.

## [0.2.0](https://github.com/trallnag/ansible-role-aws-ssm-plugin/compare/v0.1.0...v0.2.0) / 2024-07-27

### Changed

- Replaced `ansible.builtin.yum` with `ansible.builtin.dnf`.

## [0.1.0](https://github.com/trallnag/ansible-role-aws-ssm-plugin/compare/72dad404d48e94e60c03e8a311544852c7316f37...v0.1.0) / 2024-05-19

Initial release.
