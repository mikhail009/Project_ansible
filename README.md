Readme
=========
Стартовый плейбук для DEBIAN

1. Устанавливает “Zabbix-agent” и “mlocate” в “Debian”
2 .Устанавливает "Zabbix-agent" в "RedHat"
3. Добавляет “ansible” пользователя   в “Ubuntu”
4. Добавляет "ansible" пользователя  в "RedHat"
5. Устанавливает “nano”, “wget”,  “unzip”,  “traceroute”,  “mlocate",  “htop  в ”RedHat"
6. Создаёт группу “Projects” в “Debian” и  “RedHat” , создаёт папку “Projects в корне”,  выдаёт группе “Projects” полные права на папку “Projects”, делает владельцам папки "ansible"
7. Добавляет  пользователя “veeam-user” с помощью которого подключается veeam-agent и создаёт бэкапы VM при помощи хэштэгов в “Vcenter”
8. Добавляет пользователя “backuper”  с помощью которого делаются бэкапы
9. Изменяет текущий часовой пояс на Europe/Moscow
10. Так же данный playbook не будет ставить “Zabbix-agent” если в системе ранее был установлен “Zabbix-agent”  

Requirements
------------

Запускается командой #ansible-playbook -l new playbook3.yml -K 

Role Variables
--------------

Отсутсвуют

Dependencies
------------


Example Playbook
----------------
"playbook3.yml

---
- name: install fo hren
  hosts: all
  become: yes


  roles:
    - start_playbook"



Author Information
------------------

Создал Михаил Хафизов
