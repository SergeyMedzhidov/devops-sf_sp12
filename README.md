# devops-sf_sp2
- Генерируем образ в DockerHub
```diff
SergeyMedzhidov/django-pg
```
- Деплой проекта с Helm Charts:
````
$ git clone https://github.com/SergeyMedzhidov/devops-sf_sp2.git
$ cd devops-sf_sp2/charts/
$ helm upgrade --install --namespace default --values db/values.yaml mydb db
$ helm upgrade --install --namespace default --values app/values.yaml myapp app
````
Зайти в приложение можно по адресу ноды http://ip-node:5000
