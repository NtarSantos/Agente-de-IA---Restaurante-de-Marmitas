# 🤖 Atentende da Log Marmitas

![Status](https://img.shields.io/badge/status-MVP%20em%20desenvolvimento-black)
![License](https://img.shields.io/badge/license-MIT-green)
![IA](https://img.shields.io/badge/IA-OpenAI%20--4.1-yellow)
![Automation](https://img.shields.io/badge/Automation-n8n-orange)
![Database](https://img.shields.io/badge/Database-PostgreSQL-blue)
![Google Sheet](https://img.shields.io/badge/Planilha-Google%20|%20Gerenciamento|%20Pedidos-lightgreen)
![TelegramAPI](https://img.shields.io/badge/TelegramBot%20API-success-lightblue)

---

## 📘 Sobre o Projeto

A **Atendente Virtual Inteligente** é uma solução de **automação de pré-atendimento** desenvolvida para atender clientes via **Telegram** de forma **humanizada, eficiente e totalmente automática**.
O projeto visa reduzir custos operacionais e aumentar a produtividade de atendentes da Log Marmitas, utilizando **Inteligência Artificial** e **orquestração de fluxos** com **n8n**.  


---

## 🎯 Objetivo

Desenvolver uma **Atendente Virtual Inteligente** capaz de:
- Atender automaticamente clientes via Telegram;
- Informar as marmitas que o restuarante possui disponível, fechar o pedido e salvar no google sheets.
- Notifica o contato da cozinha com o resumo do pedido realizado. 
- Sistema de Recuperação de Carrinho Abandonado (Abandoned Cart Recovery), o cliente que não fechar o pedido após 10min, será relembrado/notificado.
- Operar com **baixo custo**, **alta performance** e **estrutura pronta para escalar**.

---

## 👁️‍🗨️ Testar O Agente de IA

Acessar o telegram e pesquisar pelo o bot **@ntarbotlogmanagerbot**
https://web.telegram.org/k/#@ntarbotlogmanagerbot

O gerenciamento dos pedidos ficarão salvos na **planilha do google sheet** abaixo:
https://docs.google.com/spreadsheets/d/1IQf7Cm1Mv2kP0JJz8-S-jkwFy74uq0JRIGaFubke5co/edit?usp=sharing

---

## 🧠 Tecnologias Utilizadas

| Camada | Tecnologia | Função |
|--------|-------------|--------|
| **IA** | [OpenAI – 4.1 mini](https://platform.openai.com/) | Modelo leve e super inteligente |
| **Automação** | [n8n (self-hosted)](https://n8n.io) | Orquestração de fluxos e integrações |
| **Mensageria** | [Telegram](https://web.telegram.org/k/#@ntarbotlogmanagerbot) | Envio e recebimento de mensagens Telegram |
| **Banco de Dados** | PostgreSQL | Salvar conversas e ter memória |
| **Infraestrutura** | VPS Contabo | Hospedagem do ambiente completo |
| **Gestão de Pedidos** | Google Sheets | Acompanhamento dos Pedidos |

---

## 🧱 Arquitetura do MVP

A arquitetura do Atendente Inteligente foi desenhada para ser leve, modular e escalável, garantindo baixo custo e alta performance no MVP.
Cada componente conversa entre si de forma harmônica, garantindo fluidez e autonomia no atendimento via WhatsApp.

                💬 Usuário (Telegram)
                          │
                          ▼
                🌐 Telegram API (Gateway)
                          │
                          ▼
        ⚙️ n8n (Automação + IA Maritaca)
        ├── Fluxos de automação
        ├── Regras de follow-up
        └── Interação com a IA (OpenAI 4.1 mini)
                          │
                          ▼
         🗄️ Banco de Dados (PostgreSQL)
        ├── Clientes
        ├── Mensagens
        └── Memório do atendimento
                          │
                          ▼
          ☁️ Google Sheets (Gerenciamente)
                └── Pedidos 

## 👉 Resumo da Comunicação entre os Componentes:
O usuário interage via Telegram, solicitando o pedido de Marmitas.
A API do Telegram recebe essas mensagens e repassa ao n8n.
O n8n processa os dados, aciona o modelo da OpenAI para gerar respostas inteligentes e realizar o pedido de forma humanizada.
As informações são registradas no PostgreSQL (Clientes, status, logs).

## 🚀 Arquitetura Evolutiva da Solução

- 🔹 **n8n Cloud Pro** para automações escaláveis;
- 🔹 **Banco isolado em PostgreSQL Cloud**;
- 🔹 **Portal administrativo (FastAPI ou Spring Boot)** com dashboards, controle e gerencimente de clientes e pedidos;
- 🔹 **Autenticação segura (JWT / OAuth2)** e controle de administradores;
- 🔹 **Integração com CRMs e ferramentas de marketing**;
- 🔹 **IA avançada (OpenAI / GPT-5)** para respostas mais humanas;
- 🔹 **Alta disponibilidade e escalabilidade horizontal**.

---

## 🧰 Ferramentas de Desenvolvimento

- **Visual Studio Code** — Desenvolvimento e testes de engenharia de prompt em Markdown
- **Postman / Thunder Client** — Testes de APIs
- **dbdiagram.io / Figma** — Modelagem visual
- **Azure Data Studio** — Visualização e análise do banco de dados
- **Docker Compose** — Empacotamento e deploy local do n8n e Postgres
- **API do Google Sheets** - Para permissão e manipulação de planilhas. 

---

## 🗃️ Arquitetura do DataBase

- (https://dbdiagram.io/d/Atentente_Log_Manager-69162eea6735e11170b7fa5d)

---

## 📜 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
