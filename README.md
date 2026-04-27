# ForumHub - API Rest com Spring Security

> **Projeto em Desenvolvimento**

Este projeto é uma API REST robusta desenvolvida durante o curso **"Java e Spring Security: proteja suas APIs REST"** da Alura, sob orientação da instrutora **Iasmin Araujo**. O foco principal é a implementação de segurança, autenticação e autorização em ambientes stateless.

## Objetivos do Projeto

O ForumHub é um backend para um fórum de discussões onde a segurança é aplicada em cada camada. O projeto demonstra o domínio de fluxos de autenticação modernos e proteção de endpoints.

### Principais Funcionalidades:
* **Autenticação Stateless:** Arquitetura que não armazena estado no servidor, ideal para escalabilidade.
* **Segurança com JWT:** Fluxo de autenticação baseado em tokens (JSON Web Tokens).
* **Hashing de Senhas:** Implementação de `BCryptPasswordEncoder` para armazenamento seguro de credenciais.
* **Gestão de Perfis:** Controle de acesso baseado em diferentes níveis de permissão.
* **Boas Práticas HTTP:** Tratamento de erros e retornos de códigos de status adequados (200, 201, 401, 403).
* **Persistência e Versão:** Uso de JPA/Hibernate com MySQL e controle de versão de banco com Flyway.

## Tecnologias Utilizadas

* **Java 21:** Utilizando os recursos mais recentes da linguagem.
* **Spring Boot 3.3.4:** Framework produtivo para aplicações Java.
* **Spring Security:** Framework de segurança para autenticação e controle de acesso.
* **Spring Data JPA:** Facilidade na persistência de dados.
* **MySQL:** Banco de dados relacional para armazenamento de usuários e tópicos.
* **Flyway Migration:** Ferramenta de versionamento de banco de dados.
* **Maven:** Gestão de dependências e automação de build.

## Como Rodar a Aplicação

### Pré-requisitos:
* JDK 21 instalado.
* MySQL Server configurado.
* IDE de sua preferência (IntelliJ, Eclipse, VS Code).

### Passo a Passo:
1. **Clone o repositório:**
   ```bash
   git clone https://github.com/ryanricardoo/3867-seguranca-java-3.git
   
2. **Configure o banco de dados:
No arquivo src/main/resources/application.properties, ajuste as credenciais do seu MySQL:
spring.datasource.url=jdbc:mysql://localhost:3306/forum_hub
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha

3. **Execute as Migrations:
O Flyway executará automaticamente os scripts SQL na inicialização.

4. **Inicie a aplicação:
Rode o projeto através da sua IDE ou via terminal:
```bash
   mvn spring-boot:run
