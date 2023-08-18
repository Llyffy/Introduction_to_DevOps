# Домашнее задание к занятию "`GitLab`" - `Букин Даниил`

### Задание 1
**Что нужно сделать:**

1. Разверните GitLab локально, используя Vagrantfile и инструкцию, описанные в [этом репозитории](https://github.com/netology-code/sdvps-materials/tree/main/gitlab).   
2. Создайте новый проект и пустой репозиторий в нём.
3. Зарегистрируйте gitlab-runner для этого проекта и запустите его в режиме Docker. Раннер можно регистрировать и запускать на той же виртуальной машине, на которой запущен GitLab.

В качестве ответа в репозиторий шаблона с решением добавьте скриншоты с настройками раннера в проекте.

Я развернул без использования Vagrantfile, т.к. он недоступен в россии.
Вот скриншоты работоспособности моего раннера:

1. ![image](https://github.com/Llyffy/Homework/assets/53367937/b459cd1f-5431-48a1-9f63-1436f587cd1e)

2. ![image](https://github.com/Llyffy/Homework/assets/53367937/6aedb76c-b427-46d9-a09e-94f8f385e5c9)

### Задание 2
**Что нужно сделать:**

1. Запушьте [репозиторий](https://github.com/netology-code/sdvps-materials/tree/main/gitlab) на GitLab, изменив origin. Это изучалось на занятии по Git.
2. Создайте .gitlab-ci.yml, описав в нём все необходимые, на ваш взгляд, этапы.

В качестве ответа в шаблон с решением добавьте: 
   
 * файл gitlab-ci.yml для своего проекта или вставьте код в соответствующее поле в шаблоне; 
 * скриншоты с успешно собранными сборками.

1. ![image](https://github.com/Llyffy/Homework/assets/53367937/90e4a86f-c8b6-4d61-88a3-cf1a67733fc9)

2. ![image](https://github.com/Llyffy/Homework/assets/53367937/ee741e05-7c40-4e03-a2bc-385ac74ac95f)

Вот так выглядит мой .gitlab-ci.yml
```
stages:
  - build
  - test
  - deploy

build:
  stage: build
  script:
    - echo "Building the project..."

test:
  stage: test
  script:
    - echo "Running tests..."

deploy:
  stage: deploy
  script:
    - echo "Deploying the project..."

```
