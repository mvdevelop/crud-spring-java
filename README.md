
## ☕ CRUD Spring Java

Este é um projeto de API RESTful desenvolvido com Java e Spring Boot, utilizando o banco de dados NoSQL MongoDB. 
A aplicação segue os princípios da arquitetura em camadas e boas práticas de desenvolvimento para gerenciar operações de CRUD (Create, Read, Update, Delete).

## 🚀 Tecnologias Utilizadas

Java 17+: Linguagem de programação principal.
Spring Boot 3.x: Framework para facilitar a configuração e o desenvolvimento da aplicação.
Spring Data MongoDB: Módulo para persistência de dados em banco NoSQL.
Maven: Gerenciador de dependências e automação de build.
Lombok: Biblioteca para redução de código boilerplate (Getters, Setters, etc.).
MongoDB: Banco de dados orientado a documentos.

## 🛠️ Funcionalidades

Create: Cadastro de novos registros no banco de dados.
Read: Consulta de registros por ID ou listagem completa.
Update: Atualização de dados de registros existentes.
Delete: Remoção de registros por ID.
Tratamento de Exceções: Retornos HTTP padronizados para erros de requisição.

## 📋 Endpoints da API
Abaixo estão as rotas principais da aplicação: MétodoEndpointDescrição
POST/api/users Cria um novo registro
GET/api/users Retorna todos os registros
GET/api/users/{id} Retorna um registro específico por ID
PUT/api/users/{id} Atualiza os dados de um registro
DELETE/api/users/{id} Remove um registro do banco

## 🔧 Configuração e InstalaçãoPré-requisitosJDK 17 ou superior instalado.
Maven instalado e configurado no PATH.MongoDB rodando localmente (porta 27017) ou via MongoDB Atlas.

Passo a PassoClone o repositório:
Bashgit clone https://github.com/mvdevelop/crud-spring-java.git
cd crud-spring-java
Configure o Banco de Dados:No arquivo src/main/resources/application.
properties, ajuste a URI de conexão se necessário:Propertiesspring.data.mongodb.uri=mongodb://localhost:27017/nome_do_seu_banco
Execute a aplicação:Bashmvn spring-boot:run
A API estará disponível em http://localhost:8080.

## 📁 Estrutura do ProjetoPlaintextsrc/main/java/com/projeto/

├── controllers/    # Camada de entrada (Exposição dos Endpoints REST)
├── services/       # Camada de Regras de Negócio
├── repositories/   # Camada de acesso ao MongoDB (Spring Data)
├── models/         # Definição das Entidades/Documentos
└── exceptions/     # Customização de erros e handlers

## 👨‍💻 AutorDesenvolvido por mvdevelop.
GitHub: @mvdevelopLinkedIn: Seu Nome Aqui

## 📄 LicençaEste projeto está sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.
