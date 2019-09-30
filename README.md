cloud3rsio.journald
=========

Update journald configuration.

Installation
------------

```bash
$ ansible-galaxy install cloud3rsio.journald
```

Requirements
------------

Nothing.

Role Variables
--------------

| Key | Default Value | Type |
| ------------- | ------------- | ------------- |
| `journald_Storage` | `auto` | String |
| `journald_Compress` | `'yes'` | String |
| `journald_Seal` | `'yes'` | String |
| `journald_SplitMode` | `uid` | String |
| `journald_SyncIntervalSec` | `5m` | String |
| `journald_RateLimitInterval` | `30s` | String |
| `journald_RateLimitBurst` | `1000` | Int |
| `journald_SystemMaxUse` | `500M` | String |
| `journald_RuntimeMaxUse` | `500M` | String |
| `journald_MaxFileSec` | `1month` | String |
| `journald_ForwardToSyslog` | `'yes'` | String |
| `journald_ForwardToKMsg` | `'no'` | String |
| `journald_ForwardToConsole` | `'no'` | String |
| `journald_ForwardToWall` | `'yes'` | String |
| `journald_TTYPath` | `/dev/console` | String |
| `journald_MaxLevelStore` | `debug` | String |
| `journald_MaxLevelSyslog` | `debug` | String |
| `journald_MaxLevelKMsg` | `notice` | String |
| `journald_MaxLevelConsole` | `info` | String |
| `journald_MaxLevelWall` | `emerg` | String |
| `journald_LineMax` | `48K` | String |

Dependencies
------------

Nothing.

Example Playbook
----------------

```yaml
- hosts: all
  roles:
    - role: cloud3rsio.journald
```

License
-------

[MIT](LICENSE)

Author Information
------------------

- youyo
