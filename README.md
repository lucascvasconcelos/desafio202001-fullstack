# Api REST com symfony 

## Requisitos
- Symfony
- php 7+
- composer
- PDO-pgSQL
- postgres

## Instalação
```
Clone o projeto, entre no diretório onde está localizado o projeto symfony e rode o seguinte comando:

composer install
```
## Configure sua conexão com o seu banco de dados (postgres)
```
- Crie um arquivo chamado ".env" e copie todo conteúdo do arquivo ".env.dist" para ele e altere apenas suas credenciais do db na seguinte linha:
    obs: Necessário informar a versão do banco
    DATABASE_URL=pgsql://postgres:123@127.0.0.1:5432/publicsoft?serverVersion=11.5
```

## Criação do banco e das migrações
```
php bin/console doctrine:database:create
php bin/console doctrine:migrations:migrate
```

## Levantando servidor
```
symfony server:start

- Pronto!! Sua aplicação estará disponível na porta 8000. ex: localhost:8000/enderecos
```

## O que foi feito...

```
- Criei uma estrutura de backend básica do servidor utilizando o estilo de 
arquitetura da API REST.
- Criação de um crud de endereço.
- Também foi criado uma estrutura de service para tornar o controller mais limpo.
- Separei o front do projeto em outro repositório com um projeto angular onde foi implementado o client. Segue abaixo o link do repositório com maiores informações...
```
[Repositório do front-end](https://github.com/lucascvasconcelos/endereco-api-client)

![image](https://i.ibb.co/LhLXG58/Captura-de-tela-de-2020-02-10-01-51-05.png)