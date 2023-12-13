# universa-desafio
Desafio Universa Soluções Educacionas

## Instruções para start o projeto
Requisitos docker-composer instalado

### Use docker-compose
[Docker](https://www.docker.com/) 

Para construir e iniciar a imagem, use:
```bash
$ docker-compose up -d --build
```

Para instalar a depedências do projeto use:
```bash
$ docker-compose run --rm universa composer install
```

Para construir a base de dados, use:
```bash
$ cat data/schema.sql | docker exec -i desafio sqlite3 data/db.sqlite
```