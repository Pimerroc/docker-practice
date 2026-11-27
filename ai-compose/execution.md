# Простое развертывание mistrall с ollama
Вообще тема не очень приятная для развертывания, поскольку образ ollama весит 1.5 гига, а мистрал в три раза больше. Команда все та же 
для наглядности можно даже не использовать -d флаг 
```bash
docker compose up
```

## inspect после запуска.
```bash
docker images
# processes 
docker ps
# network 
docker network ls 
# volumes
docker volume ls 
```
## manage приложения
```bash
docker compose ls
# Потом убрать комментарии с build и добавить коментарии для образов, предварительно их перед этим удалив используя rmi
docker compose up -d
# Посмотреть процессы внутри compose образов
docker compose top
```
## Cleanup
```bash
# Полная очистка, так как я не собираюсь им больше пользоваться.
docker compose down --volumes --rmi all
```


