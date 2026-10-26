# API de Produtos

API REST desenvolvida com Java e Spring Boot para praticar os fundamentos do desenvolvimento backend, incluindo operações CRUD, organização em camadas e persistência de dados com JPA.

## Tecnologias utilizadas

- Java 21
- Spring Boot
- Spring Data JPA
- Hibernate
- Oracle Database
- Maven

## Funcionalidades

A API permite realizar operações CRUD de produtos:

- Cadastrar produtos
- Listar todos os produtos
- Buscar um produto pelo ID
- Atualizar produtos
- Excluir produtos

## Endpoints

| Método HTTP | Endpoint | Descrição |
|---|---|---|
| `POST` | `/api/produtos` | Cadastrar um produto |
| `GET` | `/api/produtos` | Listar todos os produtos |
| `GET` | `/api/produtos/{id}` | Buscar um produto pelo ID |
| `PUT` | `/api/produtos/{id}` | Atualizar um produto |
| `DELETE` | `/api/produtos/{id}` | Excluir um produto |

## Organização do projeto

Organizei o projeto em camadas para separar as responsabilidades de cada parte:

- **Controller:** recebe as requisições da API.
- **Service:** contém a lógica da aplicação.
- **Repository:** responsável pelo acesso ao banco de dados.
- **Model:** representa os produtos.

## Como executar

É necessário ter o Java 21 instalado e acesso a um banco de dados Oracle.

Configure as variáveis de ambiente utilizadas no `application.properties`:

- `DB_URL`
- `DB_USERNAME`
- `DB_PASSWORD`

Depois, na pasta do projeto, execute no Windows:

```powershell
.\mvnw.cmd spring-boot:run
```
