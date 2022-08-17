Readme
=========
#### Сommon playbook

- Устанавливает “Zabbix-agent” и “mlocate” в “Debian”
- Устанавливает "Zabbix-agent" в "RedHat"
- Добавляет “ansible” пользователя   в “Ubuntu”
- Устанавливает “nano”, “wget”,  “unzip”,  “traceroute”,  “mlocate",  “htop  в ”RedHat"
- Создаёт группу “Projects” в “Debian” и  “RedHat” , создаёт папку “Projects в корне”,  выдаёт группе “Projects” полные права на папку “Projects”, делает владельцам папки "ansible"
- Добавляет  пользователя “veeam-user” с помощью которого подключается veeam-agent и создаёт бэкапы VM при помощи хэштэгов в “Vcenter”
- Добавляет пользователя “backuper”  с помощью которого делаются бэкапы
- Изменяет текущий часовой пояс на Europe/Moscow
- Так же данный playbook не будет ставить “Zabbix-agent” если в системе ранее был установлен “Zabbix-agent”  

Рекомендации
------------
Запускается командой
```ansible-playbook -l new playbook3.yml -K```


Пример Playbook
----------------
playbook3.yml
```
---
- name: install fo playbook
  hosts: all
  become: yes


  roles:
    - start_playbook
```
