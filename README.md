# Parking Control API

## Descrição
O projeto **Parking Control API** é uma API RESTful desenvolvida em Java com o framework Spring Boot. A finalidade desta API é gerenciar os dados de estacionamento, permitindo operações básicas de CRUD (Create, Read, Update, Delete) sobre os registros de vagas de estacionamento.

## Funcionalidades Principais
- Criação, leitura, atualização e exclusão de vagas de estacionamento.
- Validação de campos para evitar duplicatas e garantir a integridade dos dados.
- Consulta paginada das vagas de estacionamento.
- Suporte a diferentes endpoints para acesso aos recursos da API.

## Tecnologias Utilizadas
- Java
- Spring Boot
- Spring Data JPA
- Hibernate
- Postman
- PostgreSQL
- Maven

## Estrutura do Projeto
O projeto está dividido nas seguintes partes:

- **Controllers:** Contém os controladores responsáveis por definir os endpoints da API e mapear as requisições HTTP para os métodos apropriados.
- **Services:** Contém a lógica de negócio da aplicação, onde são realizadas as operações sobre os dados.
- **Models:** Define as entidades de dados que representam as vagas de estacionamento e seus atributos.
- **Repositories:** Contém as interfaces responsáveis pela interação com o banco de dados, utilizando o Spring Data JPA.

## Configuração e Execução
Para executar o projeto localmente, siga os passos abaixo:

1. Certifique-se de ter o Java JDK, o Maven e o PostgreSQL instalados em seu ambiente.
2. Clone o repositório do projeto em sua máquina local.
3. Configure o arquivo `application.properties` com as informações de conexão ao banco de dados PostgreSQL.
4. Execute o comando `mvn clean install` na raiz do projeto para baixar as dependências e compilar o código.
5. Execute o comando `mvn spring-boot:run` para iniciar a aplicação.
6. Acesse os endpoints da API utilizando um cliente HTTP, como Postman ou cURL.

## Endpoints da API
A API expõe os seguintes endpoints:

- **POST /parking-spot:** Cria uma nova vaga de estacionamento.
- **GET /parking-spot:** Retorna uma lista paginada de todas as vagas de estacionamento.
- **GET /parking-spot/{id}:** Retorna os detalhes de uma vaga de estacionamento específica com o ID fornecido.
- **PUT /parking-spot/{id}:** Atualiza os dados de uma vaga de estacionamento existente com o ID fornecido.
- **DELETE /parking-spot/{id}:** Exclui uma vaga de estacionamento específica com o ID fornecido.

## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir um pull request ou relatar problemas através das issues.
