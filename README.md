# 🤖 SDR Virtual Inteligente

![Status](https://img.shields.io/badge/status-MVP%20em%20desenvolvimento-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![IA](https://img.shields.io/badge/IA-OpenAI%20--4.1-yellow)
![Automation](https://img.shields.io/badge/Automation-n8n-orange)
![Database](https://img.shields.io/badge/Database-PostgreSQL-blue)
![Google Sheet](https://img.shields.io/badge/Planilha-Google%20|%20Gerenciamento|%20Pedidos-lightgrey)
![TelegramAPI](https://img.shields.io/badge/TelegramBot%20API-success)

---

## 📘 Sobre o Projeto

A **Atendente Virtual Inteligente** é uma solução de **automação de pré-atendimento** desenvolvida para atender clientes via **Telegram** de forma **humanizada, eficiente e totalmente automática**.
O projeto visa reduzir custos operacionais e aumentar a produtividade de atendentes comerciais, utilizando **Inteligência Artificial** e **orquestração de fluxos** com **n8n**.  


---

## 🎯 Objetivo

Desenvolver uma **Atendente Virtual Inteligente** capaz de:
- Atender automaticamente clientes via Telegram;
- Informar as marmitas que o restuarante possui disponível, fechar o pedido e salvar no google sheets.
- Operar com **baixo custo**, **alta performance** e **estrutura pronta para escalar**.

---

## 🧠 Tecnologias Utilizadas

| Camada | Tecnologia | Função |
|--------|-------------|--------|
| **IA** | [OpenAI – 4.1 Mini](https://platform.openai.com/) | Modelo leve e super inteligente |
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

O projeto foi construído com base **modular e escalável**, permitindo evolução natural para um ecossistema distribuído:

- 🔹 **n8n Cloud Pro** para automações escaláveis;
- 🔹 **Banco isolado em PostgreSQL Cloud**;
- 🔹 **Portal administrativo (FastAPI ou Spring Boot)** com dashboards e controle de múltiplos clientes;
- 🔹 **Autenticação segura (JWT / OAuth2)** e controle de administradores;
- 🔹 **Integração com CRMs e ferramentas de marketing**;
- 🔹 **IA avançada (OpenAI / GPT-5)** para respostas mais humanas;
- 🔹 **Alta disponibilidade e escalabilidade horizontal**.

---

---

## 🧰 Ferramentas de Desenvolvimento

- **Visual Studio Code** — Desenvolvimento e testes
- **Postman / Thunder Client** — Testes de APIs
- **dbdiagram.io / Figma** — Modelagem visual
- **Azure Data Studio** — Visualização e análise do banco de dados
- **Docker Compose** — Empacotamento e deploy local do n8n e Postgres

---

## 🗃️ Arquitetura do DataBase

- https://dbdiagram.io/d/SDR_VIRTUAL-691528c26735e111708c65ec

---

## 📜 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
