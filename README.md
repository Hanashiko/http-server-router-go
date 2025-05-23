# 📦 HTTP Server Router (Go)

Це мінімалістичний HTTP-сервер на Go, який реалізує базовий роутер без використання сторонніх бібліотек. Кожен запит маршрутизується залежно від URL-пути (`/a`, `/b`, `/c`). Для інших шляхів повертається 404.

## 🧠 Опис

Цей проєкт показує, як реалізувати інтерфейс `http.Handler` через власний тип `router`, що дозволяє обробляти HTTP-запити вручну.

## 🚀 Запуск

1. Клонуйте репозиторій або скопіюйте код.
2. Запустіть сервер:

```bash
go run main.go
```

3. Відкрийте браузер або використайте `curl`:

```bash
curl http://localhost:8000/a
# Output: Executing /a

curl http://localhost:8000/unknown
# Output: 404 Not Found
```

## 📌 Примітки

- Цей роутер призначений для демонстраційних або навчальних цілей.
- Для складніших рішень рекомендується використовувати фреймворки на кшталт [Gorilla Mux](https://github.com/gorilla/mux) або [Chi](https://github.com/go-chi/chi).
