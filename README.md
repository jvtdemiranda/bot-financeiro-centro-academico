# 🏫 Controle Financeiro pelo Telegram

Chega de planilhas complicadas! Com esse bot você registra 
entradas e saídas financeiras direto pelo Telegram em segundos 
— sem precisar abrir nenhum sistema.

## 💡 Qual problema resolve?

Organizações como centros acadêmicos, associações e pequenos 
negócios perdem tempo tentando manter o controle financeiro 
atualizado. Esse bot simplifica tudo isso numa conversa de Telegram.

## ✅ O que você consegue fazer

- Registrar uma entrada ou saída em segundos
- Consultar o saldo atual a qualquer momento
- Acessar o histórico completo na planilha com um clique
- Tudo isso sem instalar nada — só pelo Telegram

## 📱 Como funciona na prática

O usuário envia uma mensagem simples como:
- `entrada 150,00 - Taxa de inscrição`
- `saida 80,00 - Compra de material`
- `saldo`

E o bot registra, confirma e mantém tudo organizado automaticamente.

## 🔄 Fluxo da automação

Telegram Trigger
↓
Code Python (interpreta a mensagem)
↓
Switch (direciona pelo tipo)
↓
├── /start → Menu de boas vindas
├── entrada → Google Sheets → Confirmação
├── saida  → Google Sheets → Confirmação
├── saldo  → Google Sheets → Cálculo → Resposta + Link
└── erro   → Mensagem orientando o usuário

## 🛠️ Tecnologias utilizadas

- [n8n](https://n8n.io) — automação de fluxos
- Telegram Bot API
- Google Sheets API
- Python (nós de código)

## 💬 Comandos do bot

| Comando | Descrição |
|---|---|
| `/start` | Exibe o menu de boas vindas |
| `entrada 150,00 - Descrição` | Registra uma entrada |
| `saida 80,00 - Descrição` | Registra uma saída |
| `saldo` | Exibe o saldo atual |

## 🚀 Como usar

1. Importe o arquivo `workflow.json` no n8n
2. Configure as credenciais do Telegram e Google Sheets
3. Ative o workflow
4. Pronto!

## 👨‍💻 Autor

João Vitor — [github.com/jvtdemiranda](https://github.com/jvtdemiranda)
