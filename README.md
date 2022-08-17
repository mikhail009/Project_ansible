Readme
=========
Стартовый плейбук для DEBIAN

Устанавливает “Zabbix-agent” и “mlocate” в “Debian”
Устанавливает "Zabbix-agent" в "RedHat"
Добавляет “ansible” пользователя   в “Ubuntu”
Добавляет "ansible" пользователя  в "RedHat"
Устанавливает “nano”, “wget”,  “unzip”,  “traceroute”,  “mlocate",  “htop  в ”RedHat"
Создаёт группу “Projects” в “Debian” и  “RedHat” , создаёт папку “Projects в корне”,  выдаёт группе “Projects” полные права на папку “Projects”, делает владельцам папки "ansible"
Добавляет  пользователя “veeam-user” с помощью которого подключается veeam-agent и создаёт бэкапы VM при помощи хэштэгов в “Vcenter”
Добавляет пользователя “backuper”  с помощью которого делаются бэкапы
Изменяет текущий часовой пояс на Europe/Moscow
Так же данный playbook не будет ставить “Zabbix-agent” если в системе ранее был установлен “Zabbix-agent”  

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
playbook3.yml

---
- name: install fo hren
  hosts: all
  become: yes


  roles:
    - start_playbook


License
-------

BSD

Author Information
------------------

Создал Михаил Хафизов
