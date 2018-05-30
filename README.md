# ansible-role-traditional-desktop

Ensure a traditional desktop enviroment (gnome 2/mate) is installed on RHEL/Ubuntu. e.g.

- RHEL 6: Gnome 2 is installed
- RHEL 7: MATE/GNOME is installed
- Ubuntu: MATE is installed from the universe repository

## Requirements

None

## Role Variables

| Variable Name             | Defaults | Description                                            |
|---------------------------|----------|--------------------------------------------------------|
| headless                  |False     | If true, the display manager/gui init will be disabled |
| remove_gnome_3            |False     | If true, removes gnome 3 where present                 |

## Dependencies

gabethecabbage.elrepo

## Example Playbook

    ---
    - hosts: servers
      roles:
        - role: dfgd.MateGnome-desktop
    ...

## License

BSD

## Author Information

Changed by [dfgd](https://github.com/dfgd).

Forked role from[Gabe Schrecker](https://github.com/gabethecabbage).

