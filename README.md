# Golang + GORM + Mux

Configuração base de um projeto Golang

### Pré-requisitos
 - Docker instalado e configurado

### Instalação
Assume que atenda aos pré-requisitos informados acima para seguir com os passos abaixo:

Clonar repositório
```sh
$ git clone https://github.com/edujudici/go-quest.git
```

Running database local
```sh
$ docker run --name postgres_db  -p 5432:5432 -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=postgres -e POSTGRES_DB=quests -d postgres
```

Running application
```sh
$ go run main.go
```

### Collection
```sh
POST: http://localhost:8008/quests
PUT: http://localhost:8008/quests/id
DELETE: http://localhost:8008/quests/id
GET: http://localhost:8008/quests/id
GET: http://localhost:8008/quests
```


License
----

MIT

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)
