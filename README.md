# Демо
- Сборка на golang:alpine
- Запуск на scratch из собранного bin

Сборка следующей командой:
```bash
CGO_ENABLED=0 GOOS=linux GOARCH=amd64 go build
```

Клонируем репозиторий git clone

запускаем сборку image - $ docker build -t go-api:latest .

проверка $ docker images

запускаем контейнер $ docker run --name go-api-demo -d go-api

проверка $ docker ps 
