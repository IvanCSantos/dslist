# API de Games - Intensivão Java Spring Boot

Projeto desenvolvido durante o Intensivão Java Spring Boot promovido pela DevSuperior, com uma semana de estudos intensivos sobre Java Spring Boot.

## 📚 Sobre o projeto
Esta aplicação foi criada como parte das atividades práticas de um bootcamp intensivo, com foco no desenvolvimento de APIs REST utilizando Java com o framework Spring Boot.

Durante o projeto, foram abordados conceitos fundamentais de desenvolvimento backend em Java, organizando a aplicação em camadas bem definidas:
•	Controller – Responsável por expor os endpoints da API.
•	Service – Responsável pela lógica de negócio.
•	Repository – Responsável pela comunicação com o banco de dados.

⚙️ Tecnologias e Ferramentas Utilizadas
- Java 17
- Spring Boot
- Spring Data JPA
- Banco de dados H2 (ambiente de desenvolvimento)
- PostgreSQL (ambiente de produção)
- Docker (para containerização da aplicação)

## 🚀 Objetivos do Projeto
- Praticar os conceitos fundamentais do Spring Boot.
- Aplicar boas práticas de organização em camadas.
- Utilizar banco de dados relacional com JPA/Hibernate.
- Criar um ambiente pronto para produção com Docker e PostgreSQL.

## 🌐 Acesso à aplicação em produção
A aplicação está disponível no seguinte endereço:

🔗 https://gameapi.ivansantos.dev

📌 Endpoints Disponíveis
- GET /games
Retorna a lista de todos os games cadastrados.
- GET /games/{id}
Retorna as informações completas de um game específico, com base no seu ID.
- GET /lists
Retorna todas as listas de games.
- GET /lists/{id}
Retorna os detalhes de uma lista específica, com base no seu ID.
- GET /lists/{id}/games
Retorna os games associados a uma lista específica, com base no ID da lista.

## 🛠️ Como executar o projeto
### 🗃️ Preparar o Banco de Dados
1.	Localize o arquivo create.sql na raiz do projeto.
2.	Execute esse script no banco PostgreSQL para criar a tabela e importar os registros iniciais.

Você pode fazer isso diretamente pelo PgAdmin ou utilizando uma ferramenta de linha de comando como psql.

⸻

### 🐳 Subir os containers da aplicação

Com Docker e Docker Compose instalados, execute o seguinte comando na raiz do projeto:

```declarative
docker compose up -d
```

Esse comando irá iniciar os containers do PostgreSQL e do PgAdmin.

### 🌐 Acessar o PgAdmin

Após a execução, acesse o PgAdmin através do navegador:

🔗 http://localhost:5050

Use as credenciais abaixo para login:
- Usuário: me@example.com
- Senha: 1234567

Obs.: Após o login, você pode adicionar uma nova conexão apontando para o container do PostgreSQL com as configurações definidas no docker-compose.yml.