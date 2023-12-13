# Desafio para Universa Soluções Educacionas

## Instruções para iniciar o desafio
Requisitos docker-composer instalado

### Use docker-compose
[Docker](https://www.docker.com/) 

Para construir a imagem, use:
```bash
$ docker-compose up -d --build
```

Instalar as dependências do desafio:
```bash
$ docker-compose run --rm universa composer install
```

Para iniciar a base de dados:
```bash
$ cat data/schema.sql | docker exec -i desafio sqlite3 data/db.sqlite
```
