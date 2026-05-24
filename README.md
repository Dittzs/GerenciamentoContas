# GerenciamentoContas
Software de gerenciamento de contas rodando em server.js

# KatarinaJob — Smurfs Manager

## Como instalar e rodar

### 1. Instale o Node.js (se não tiver)
Baixe em: https://nodejs.org  
Versão recomendada: **LTS (20.x ou superior)**

### 2. Coloque os arquivos numa pasta
Estrutura:
```
katarinajob/
  server.js
  index.html
```

### 3. Inicie o servidor
Abra o terminal (Prompt de Comando ou PowerShell) dentro da pasta e rode:
```
node server.js
```

Você verá:
```
✅  KatarinaJob rodando em http://localhost:3000
```

### 4. Abra no navegador
Acesse: **http://localhost:3000**

---

## Por que precisa do servidor?

A Riot API bloqueia chamadas diretas do navegador (CORS).  
O `server.js` funciona como um proxy local que faz as chamadas pela sua máquina, contornando esse bloqueio.

---

## Configuração inicial

1. Acesse **https://developer.riotgames.com**, faça login e gere uma **API Key**
2. Cole a chave no campo **RIOT API KEY** — ela fica **salva automaticamente**
3. Selecione a região (**BR** já é o padrão)
4. Digite o nick no formato **Nome#TAG** → pressione Enter → elo e PDL aparecem na hora

---

## Auto-atualização

Ative o toggle **Auto-atualizar** e escolha o intervalo (1 min, 5 min, 10 min, etc).  
A planilha se atualiza sozinha sem você precisar fazer nada.

---

## Para deixar rodando sempre (Windows)

Crie um arquivo `iniciar.bat` com:
```bat
@echo off
node "C:\caminho\para\katarinajob\server.js"
pause
```
Coloque um atalho na pasta **Inicialização** do Windows para iniciar junto com o PC:  
`Win + R` → `shell:startup` → cole o atalho do .bat lá.

---

## API Key expirou?

- **Development Key**: dura 24h, gratuita, renovável no site
- **Production Key**: permanente, requer aprovação da Riot (formulário no developer portal)
