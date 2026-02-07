# 📧 Email Service API – Backend Challenge (Uber Style)

Este projeto é uma **API REST desenvolvida em Java com Spring Boot**, criada como solução para um **desafio técnico de backend**, inspirado em desafios reais aplicados por empresas como a Uber.

O objetivo é fornecer um serviço simples, bem estruturado e escalável para **envio de e-mails**, seguindo boas práticas de arquitetura backend.

---

## 🚀 Funcionalidades

- Endpoint REST para envio de e-mails
- Arquitetura em camadas (Controller, Service, DTO)
- Separação clara de responsabilidades
- Estrutura preparada para integração com serviços externos (ex: AWS SES)
- API orientada a boas práticas REST

---

## 🛠️ Tecnologias Utilizadas

- Java 17  
- Spring Boot  
- Spring Web  
- Maven  
- Lombok  
- Postman (testes de API)

---

## 📁 Estrutura do Projeto
src/main/java/com/seunome/emailservice
│
├── controller
│ └── EmailController.java
│
├── service
│ ├── EmailService.java
│ └── EmailServiceImpl.java
│
├── dto
│ └── EmailRequestDTO.java
│
├── exception
│ └── EmailSendException.java
│
└── EmailServiceApplication.java


---

## 👨‍💻 Autor

Desenvolvido por João Victor
📌 Projeto criado para fins de aprendizado, portfólio e desafios técnicos backend.

---

## 📡 Endpoints Disponíveis

### ➤ Enviar e-mail

**POST** `/api/email/send`

#### Request Body (JSON)
```json
{
  "to": "destinatario@email.com",
  "subject": "Assunto do e-mail",
  "body": "Conteúdo do e-mail"
}

Response

204 No Content → e-mail processado com sucesso

## Como Executar o Projeto
# Pré-requisitos

Java 17+
Maven
Passos

# Clonar o repositório
git clone https://github.com/joaodddev/email-serviceapi-java.git

# Entrar no diretório
cd email-service

# Rodar a aplicação
mvn spring-boot:run


A API ficará disponível em:

http://localhost:8080
