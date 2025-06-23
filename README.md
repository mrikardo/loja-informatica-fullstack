# Loja de Informática Fullstack

Projeto completo de loja de informática com backend em Node.js + MongoDB e frontend em React.

## Como rodar localmente com Docker

```bash
docker-compose up --build
```

O backend ficará disponível em http://localhost:3000  
O frontend em http://localhost:8080

## Variáveis de ambiente

- MONGO_URI: string de conexão com MongoDB
- JWT_SECRET: segredo para geração de tokens JWT
- REACT_APP_API_URL: URL do backend para o frontend consumir (ex: http://localhost:3000)

## Deploy

### Backend no Render

- Crie um serviço Node.js no Render usando a pasta backend.
- Configure as variáveis MONGO_URI e JWT_SECRET no painel do Render.
- Comando de build: `npm install`
- Comando start: `node server.js`

### Frontend no Vercel

- Crie um projeto React no Vercel usando a pasta frontend.
- Configure a variável REACT_APP_API_URL apontando para a URL do backend no Render.