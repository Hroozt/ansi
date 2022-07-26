# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?


**group_vars\all\example.yml**


2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?


**ansible-playbook -i inventory/test.yml site.yml**


3. Какой командой можно зашифровать файл?


**ansible-vault encrypt examp.yml**


4. Какой командой можно расшифровать файл?


**ansible-vault decrypt examp.yml**


5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?


**ansible-vault view examp.yml**


6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?


**ansible-playbook -i inventory/prod.yml  --ask-vault-pass  site.yml**


7. Как называется модуль подключения к host на windows?


**WinRM или psrp(PowerSHell)**


8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh


**ansible-doc --type connection -l | grep ssh  \  ansible-doc --type connection ssh**


9.  Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?


**- remote_user**

`User name with which to login to the remote server, normally set by the remote_user keyword.
If no user is supplied, Ansible will let the SSH client binary choose the user as it normally.
[Default: (null)]`
