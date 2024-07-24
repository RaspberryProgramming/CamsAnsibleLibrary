# CamsAnsibleLibrary
Custom library of ansible playbooks and other related files.

## Projects

### Local Maintenance

Library of playbooks that are meant for maintenance related to my local network

You can schedule these playbooks using cron. See example cron file below

```cron
# m h  dom mon dow   command

0 2 * * 0 ansible-playbook reboot_playbook.yml
0 1 * * * ansible-playbook updates_playbook.yaml
```

### Request Mirror

Library of playbooks for deploying request mirror project to a server. You can find the project at [https://github.com/RaspberryProgramming/request-mirror/](https://github.com/RaspberryProgramming/request-mirror/blob/test-ansible/templates/index.html.hbs)

This playbook will create a new user, install needed software, clone and build the project, and setup services for it to run under.

This playbook is also designed and tested with ubuntu, other distros may not work.