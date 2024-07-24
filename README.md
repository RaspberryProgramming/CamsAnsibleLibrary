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