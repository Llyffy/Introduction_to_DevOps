# Домашнее задание к занятию "`GitLab`" - `Букин Даниил`

### Задание 1

Вот скриншоты работоспособности моего раннера:

1. ![image](https://github.com/Llyffy/Homework/assets/53367937/b459cd1f-5431-48a1-9f63-1436f587cd1e)

2. ![image](https://github.com/Llyffy/Homework/assets/53367937/6aedb76c-b427-46d9-a09e-94f8f385e5c9)

### Задание 2

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
