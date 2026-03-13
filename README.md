Ansible Multi-Node Web Cluster

Автоматическое развёртывание:
- 2 веб-сервера Nginx
- 1 HAProxy Load Balancer
- Управление с отдельного Control Node

### Как запустить
1. Подготовь 4 Debian/Ubuntu VM, + SSH-ключи
2. Создать пользователя "secret" на нодах, или изменить пользователя в файле ansible.cfg
3. Замени IP в `inventory/hosts`
4. Запуск из корня, "ansible-playbook playbooks/site.yml"

### Скриншоты:
1. Вывод ansible-playbook
  ![Playbook](https://github.com/wudbills/Ansible-node-cluster/blob/main/playbook.PNG)
2. `http://IP_lb` в браузере (с разными серверами при обновлении)
  ![web1](https://github.com/wudbills/Ansible-node-cluster/blob/main/web1.PNG)
  ![web2](https://github.com/wudbills/Ansible-node-cluster/blob/main/web2.PNG)
