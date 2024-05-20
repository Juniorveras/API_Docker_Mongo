AngularAspNetCore-MongoDB-Docker
Criação de um projeto com Front em Angular, Back em Asp.Net Core, DB Mongo com Docker. Aplicando as boas praticas.

Execução por linha de comando Docker - docker exec -it IDCONTAINER /bin/bash -> com isso iremos entrar na raiz do container.

localhost:5000/swagger/index.html

Visual Studio 2022 - .Net 6 C# 10 / Visual Code - Angular

Para Execução do projeto Front-End Angular

Criar porta Default com o comando em linha de comando no Visual Code: ng serve --open

Os projetos em Angular estão reconhecendo a Rota com isso basta subir com o comando acima.

JWT - foi implementado no intuito de administrar os Microserviços dentro a Auth.

User: admin Pass: 1010

Dependencias: AutoMapper 10.1.1 AutoMapper.Extensions.Microsoft.DependencyInjection 8.1.1 MongoDB.Bson 2.14.1 MongoDB.Driver 2.13.2 Swashbuckle.AspNetCore 6.2.3

Docker com MongoDB:

Baixar a Imagem do MongoDB no Docker execute o comando abaixo no seu terminal: docker pull tutum/mongodb

Criação de servidor especificando uma senha: execute o comando abaixo no seu terminal: docker run -d -p 27017:27017 -p 28017:28017 -e MONGODB_PASS="MINHA SENHA" tutum/mongodb

Criando sem especificar uma senha: execute o comando abaixo no seu terminal: docker run -d -p 27017:27017 -p 28017:28017 -e AUTH=no tutum/mongodb

Caso seja implementado com criação de SENHA, ajustar os parametros de entrada no PROJETO, Appsettings.json

O próximo passo será subir o seu servidor mongo. Para isso, execute os passos abaixo: execute o comando abaixo no seu terminal: docker ps -a

Acesso ao DB com o ROBO 3T: https://blog.robomongo.org/robo-3t-1-4/

Inserir como INSERT na Collection no ROBO 3T

Insert no arquivo API.Json
