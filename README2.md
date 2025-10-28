# Аналитика и подготовка
Проект у нас написан на Golang и использует базу данных PostgreSQL

Для сборки проекта на Golang нам нужны 2 файла:
- go.mod - Описывает прогу (имя, версия Go, зависимости)
- go.sum - Хэши зависимостей
  
Я их сгенерировал отдельно и положил в проект.
дерево проекта выглядит слудющим образом
зависимости в go.mod появились после `go get github.com/jackc/pgx/v5`, соответственно в go.sum записались их хэши
```
habit-app
    ├── docker-compose.yml
    ├── Dockerfile
    ├── habits-tracker
    │   ├── cmd
    │   │   └── server
    │   │       └── main.go
    │   ├── go.mod
    │   ├── go.sum
    │   ├── init.sql
    │   └── internal
    │       ├── auth
    │       │   └── auth.go
    │       ├── handlers
    │       │   └── handlers.go
    │       ├── models
    │       │   └── models.go
    │       └── templates
    │           ├── base.html
    │           ├── habit_form.html
    │           ├── habits.html
    │           ├── login.html
    │           ├── register.html
    │           └── report.html
    ├── image.png
    └── README.md
```
