# This role enables users to install and configure chrony on their hosts.
![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

## Requirements

None

## Role Variables

| Variable | Required | Default | Comments |
|----------|----------|---------|----------|
| `chrony_pkg_state` | No | `present` | Set pkg `enabled`, `disabled`, `latest`  |
| `chrony_service_state` | No | `started` | Set service state, started, enabled or disabled  |
| `chrony_service_enabled` | No | `yes` | A list of NTP servers to use.  |
| `chrony_config_server` | No | `["0.pool.ntp.org","1.pool.ntp.org","2.pool.ntp.org", "3.pool.ntp.org"]` | A list of NTP servers to use.  |
| `chrony_config_logdir` | No | `/var/log/chrony` | A list of NTP servers to use.  |
| `chrony_timezone` | No | `Etc/UTC` | Set the timezone for your server. |

## Examples

1) Install chrony and use the default settings.

```

- hosts: all
  roles:
    - role: nholuong.chrony
```

2) Install chrony and use custom servers.

```

- hosts: all
  roles:
    - role: nholuong.chrony
  vars:
    chrony_config_server:
      - 0.pool.ntp.org
      - 2.pool.ntp.org
```

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟
