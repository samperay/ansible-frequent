# adhoc ansible commands

Simple play or oneliners would be very much helpful using the ansible adhoc commands.

```
ansible test -i hosts -m ping
ansible all -m ping
ansible localhost -m ping
ansible test -i hosts -m command -a uptime -o
ansible test -i hosts -m command -a 'cat /etc/motd' -u vagrant -o
ansible test -i hosts -m copy -a 'content="Managed by Ansible" dest=/etc/motd'
ansible test -i hosts -m command -a 'cat /etc/motd'
```
