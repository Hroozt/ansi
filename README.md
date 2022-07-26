# Самоконтроль выполненения задания
2
​
3
1. Где расположен файл с `some_fact` из второго пункта задания?
4
    **group_vars\all\example.yml**
5
​
6
2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?
7
    **ansible-playbook -i inventory/test.yml site.yml**
8
​
9
3. Какой командой можно зашифровать файл?
10
    **ansible-vault encrypt examp.yml**
11
​
12
4. Какой командой можно расшифровать файл?
13
    **ansible-vault decrypt examp.yml**
14
​
15
5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?
16
    **ansible-vault view examp.yml**
17
​
18
6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?
19
    **ansible-playbook -i inventory/prod.yml  --ask-vault-pass  site.yml**
20
​
21
7. Как называется модуль подключения к host на windows?
22
    **WinRM или psrp(PowerSHell)**
23
​
24
8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh
25
    **ansible-doc --type connection -l | grep ssh  \  ansible-doc --type connection ssh**
26
​
27
9.  Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?
28
    **- remote_user**
29
​
30
        User name with which to login to the remote server, normally set by the remote_user keyword.
31
        If no user is supplied, Ansible will let the SSH client binary choose the user as it normally.
32
        [Default: (null)]`
33
