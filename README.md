
# Setup Docker Para Projetos PHP 7.4

### Passo a passo
Abra o terminal na maquina WSL 2 e Clone Repositório
```sh
https://github.com/jadirbento/setup-docker-php74.git nome-do-projeto
```

Entre no diretório do projeto
```sh
cd nome-do-projeto
```

Abra o projeto no VS Code  

-Alterar o arquivo [.env] nome do projeto  

-Alterar o arquivo [docker-compose] nome da rede  

-Alterar o arquivo [docker-compose] número da porta nginx  

-Alterar o arquivo [docker-compose] número da porta mysql  

```sh
code .
```

Suba os containers do projeto
```sh
docker-compose up -d
```

Acessar o container (para executar comandos do Composer, exemplo: composer init)
```sh
docker-compose exec app bash
```


Instalar as dependências do projeto
```sh
composer install
```


Acessar o projeto
[http://localhost:8083](http://localhost:8083)
