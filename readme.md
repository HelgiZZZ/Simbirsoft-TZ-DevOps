# Тестовое задание DevOps

## Краткое руководство по установке приложения Flaskex

---

Системные требования:
* Ubuntu 18.04
* Docker
* Ansible
* Git


---

### Тестовое задание №1: Запуск контейнера Docker
#### Создаем image:

`cd /TZ1 && \ docker build .`

#### Находим IMAGE ID:
`docker ps`

#### Выполняем запуск контейнера:
`docker run -it -d -p 8000:5000 "IMAGE ID"`

#### В браузере вводим URL:
`http://localhost:8000/`

---

### Тестовое задание №2: Автоматическая установка приложения через Ansible

#### Запуск playbook:
`cd TZ2 && \ ansible-playbook -i hosts flaskex.yml`

#### В браузере вводим URL:
`http://localhost:5000/`

---

