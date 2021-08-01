# raspotify Ansible Role

The unofficial ansible role for installing and configuring [dtcooper's](https://github.com/dtcooper) [raspotify](https://github.com/dtcooper/raspotify).


## Requirements

This role is only compatible with those devices outlined in the [raspotify](https://github.com/dtcooper/raspotify). This is currently limited to Raspberry Pi.

## Role Variables

For more details on these configuration variables see <https://github.com/dtcooper/raspotify#configuration>

| Variable Name | Default |
| -- | -- |
| device_name | `null` |
| bitrate | `160` |
| options | `null` |
| volume_args | `null` |
| cache_args | `null` |
| backend_args | `null` |


## Dependencies

N/A

## Example Playbook

```yaml
roles:
  - role: raspotify
    vars:
      device_name: speaker
      bitrate: 320
      options: "--username <USERNAME> --password <PASSWORD>"
```

## License

MIT
