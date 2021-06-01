# shellcheck

This role enables to install [shellcheck](https://www.shellcheck.net/) on a system.

## Requirements

No requirements.

## Role Variables

| Name                    | Type   | Location            | Description                                                                                           |
| ----------------------- | ------ | ------------------- | ----------------------------------------------------------------------------------------------------- |
| shellcheck_version      | string | `defaults/main.yml` | The version of shellcheck to install. Defaults to `0.7.2`.                                            |
| shellcheck_releases_url | string | `defaults/main.yml` | The base URL of shellcheck releases repository. Defaults to `https://github.com/koalaman/shellcheck`. |
| shellcheck_os           | string | `defaults/main.yml` | The OS distribution of shellcheck to install. Defaults to `linux`.                                    |
| shellcheck_arch         | string | `defaults/main.yml` | The arch distribution of shellcheck to install. Defaults to `x86_64`.                                 |
| shellcheck_executable   | string | `vars/main.yml`     | The local path where to install shellcheck executable. Defaults to `/usr/local/sbin/shellcheck`.      |

## Dependencies

No dependencies.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- hosts: servers
  roles:
    - { role: julb.shellcheck }
```

## License

MIT

## Author Information

More to find on my [Github](https://github.com/julb).

## Contributing

This project is totally open source and contributors are welcome.

When you submit a PR, please ensure that the syntax has been checked.
