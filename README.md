# ☁️ Azure Serverless Labs

![Azure](https://img.shields.io/badge/Azure-Serverless-blue?logo=microsoftazure)
![Functions](https://img.shields.io/badge/Azure%20Functions-Event%20Driven-purple)
![.NET](https://img.shields.io/badge/.NET-8.0-512BD4?logo=dotnet)
![Architecture](https://img.shields.io/badge/Architecture-Event%20Driven-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 🚀 Visão Geral

O **Azure Serverless Labs** é um projeto prático utilizando **Azure Functions** com arquitetura **serverless orientada a eventos**, integrando serviços como Blob Storage, Service Bus e Azure SQL Database.

O objetivo é simular um backend moderno, escalável e desacoplado, seguindo padrões reais de sistemas em produção.

---

## ⚙️ Stack Tecnológica

- .NET 8 / C#
- Azure Functions
- Azure Blob Storage
- Azure Service Bus
- Azure SQL Database
- Timer Trigger (Scheduler)
- Visual Studio / VS Code
- Git & GitHub

---

## 📁 Estrutura do Projeto

azure-serverless-labs/
|
|-- fn-input-blob/
│   └── BlobProcessorFunction.cs
│
├── fn-ler-sb/
│   └── ServiceBusConsumerFunction.cs
│
├── fn-save-sql/
│   └── SqlPersistenceFunction.cs
│
├── fn-simples/
│   └── HttpTriggerFunction.cs
│
├── fn-tempo/
│   └── ScheduledTaskFunction.cs
│
└── host.json
---

## ⚙️ Funções

### 🟦 fn-input-blob
Executada automaticamente ao detectar upload no Azure Blob Storage.

- Processa arquivos enviados
- Executa lógica baseada em eventos
- Ideal para pipelines de dados

---

### 🟨 fn-ler-sb
Responsável por consumir mensagens do Azure Service Bus.

- Processamento assíncrono
- Comunicação entre sistemas
- Arquitetura desacoplada

---

### 🟩 fn-save-sql
Persistência de dados no Azure SQL Database.

- Inserção de dados estruturados
- Validação de payload
- Integração com backend

---

### 🟪 fn-simples
Função HTTP básica para testes.

- Health check da aplicação
- Validação de deploy
- Endpoint simples

---

### 🟥 fn-tempo
Função executada automaticamente por agendamento.

- Jobs automáticos
- Rotinas de manutenção
- Processos recorrentes

---

## 🔄 Fluxo de Dados

- HTTP → fn-simples  
- Blob Upload → fn-input-blob  
- Service Bus → fn-ler-sb  
- Processamento → fn-save-sql  
- Scheduler → fn-tempo  

---

## 💡 Conceitos Aplicados

- Serverless Architecture
- Event-driven design
- Microservices desacoplados
- Escalabilidade automática
- Integração de serviços cloud
- Pay-per-use model

---

## 📊 Resultado

Projeto demonstra um ecossistema completo de backend serverless na Azure, simulando cenários reais de produção com eventos, filas e persistência em banco de dados.

---

## 🏁 Conclusão

Este laboratório reforça conhecimentos em arquitetura moderna cloud, com foco em escalabilidade, baixo custo e alta eficiência operacional.
