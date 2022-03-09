# Тестовое задание 3 #
Использование циклов и vault

## Предварительные условия ##
* Запущена ВМ с Centos 7
* На ВМ добавлен SSH - ключ родительской машины
* В файл `deploy/inventory.yml` добавлены адрес и порт SSH целевой виртуальной машины
* На родительской машине (или на ВМ от которой будет происходить управление)
  * установлен Ansible

## Запуск ##
```console
ansible-playbook ./deploy/deploy.yml -i ./deploy/inventory.yml
--vault-password-file ./vault-pass.txt```