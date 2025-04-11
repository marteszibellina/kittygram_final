#  Финальное задание от Яндекс.Практикума по работе с Django REST Framework, Docker и работе на удалённом сервере.
---
## Задание прошло проверку и было принято
---

## Что было сделано

1. Апробировано использование Docker и docker-compose для автоматичкеского разворачивания проекта, его сборки и отправки на DockerHub.
2. Был настроен запуск проекта Kittygram в контейнерах и CI/CD с помощью GitHub Actions.

## Работа проекта была проверена с помощью автотестов

1. В корне репозитория был создан файл tests.yml со следующим содержимым:
```yaml
repo_owner: ваш_логин_на_гитхабе
kittygram_domain: полная ссылка (https://доменное_имя) на проект Kittygram
dockerhub_username: ваш_логин_на_докерхабе
```

2. Было скопировано содержимое файла `.github/workflows/main.yml` в файл `kittygram_workflow.yml` в корневой директории проекта.

Локальный тесты проводились в виртуальном окружении через `pytest`.

## Проверенный чек-лист.

- Проект Kittygram доступен по доменному имени, указанному в `tests.yml`.
- Пуш в ветку main запускает тестирование и деплой Kittygram, а после успешного деплоя вам приходит сообщение в телеграм.
- В корне проекта есть файл `kittygram_workflow.yml`.
