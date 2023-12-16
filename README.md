### Создание посредника (middleware) используя фреймворк Echo для Go

Подсчет количеств дней оставшихся до 1 января 2025 года и отвечает кодом состояния HTTP 200 OK.

Посредник проверяет наличие HTTP-заголовка `User-Role` и содержит `admin` и выводит на консоль `Успешно`.

## Запуск

```shell
go run github.com/Mr-Ereke/go_echo-middleware/cmd/test-task
```

## Проверка

```shell
curl --location --request GET '127.0.0.1:8080/status' \
--header 'User-Role: admin'
```
