# ROZAS CASH — app mobile (React Native + Node.js)

Projeto de demonstração inspirado no layout do vídeo enviado, sem integração com banco real e sem movimentação financeira real.

## Stack
- Frontend: React Native + Expo
- Backend: Node.js + Express
- Banco: SQLite
- Autenticação: JWT
- Senhas: bcrypt

## Estrutura
- `frontend/` — aplicativo mobile
- `backend/` — API REST

## Como executar

### 1. Backend
```bash
cd backend
npm install
npm run dev
```

A API ficará em `http://localhost:3000`.

### 2. Frontend
Em outro terminal:
```bash
cd frontend
npm install
npx expo start
```

Para testar no celular, instale o Expo Go e escaneie o QR Code.

### Android emulator
Se estiver usando o emulador Android, o frontend já usa `10.0.2.2` para acessar o computador.

### Celular físico
Abra `frontend/src/config.js` e troque `API_URL` pelo IP local do computador, por exemplo:
`http://192.168.0.10:3000`

## Funcionalidades
- Tela inicial
- Cadastro de usuário
- Login
- Sessão persistida no aparelho
- Tela principal com saldo demonstrativo
- Ações PIX, boletos e extrato
- Logout
- API protegida com JWT
- Banco SQLite criado automaticamente

> Este projeto é apenas uma demonstração educacional. Não use para guardar dinheiro real, dados bancários reais ou senhas reais.
