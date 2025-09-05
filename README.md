# Nexora/CodeDock

Uma plataforma de desenvolvimento de código alimentada por IA que permite criar projetos através de prompts em linguagem natural.

## 🚀 Funcionalidades

- **Geração de Código por IA**: Use prompts em linguagem natural para gerar projetos completos
- **Editor Integrado**: Monaco Editor com syntax highlighting
- **Preview em Tempo Real**: Visualize seu projeto rodando instantaneamente
- **WebContainer**: Execução de código diretamente no navegador
- **Templates Inteligentes**: Suporte automático para React e Node.js
- **Terminal Integrado**: Execute comandos diretamente na interface
- **Chat Follow-up**: Continue conversando com a IA para refinar seu projeto

## 🛠️ Tecnologias

### Backend
- Node.js + Express + TypeScript
- Groq SDK para processamento de linguagem natural
- CORS configurado para múltiplos domínios

### Frontend
- React + TypeScript + Vite
- TailwindCSS para styling
- Monaco Editor para edição de código
- WebContainer API para execução no navegador
- Framer Motion para animações
- Solana Wallet Adapter

## 📦 Instalação e Execução

### Pré-requisitos
- Node.js 18+
- npm ou pnpm

### Configuração

1. **Clone o repositório**
```bash
git clone <repository-url>
cd nexora-codedock
```

2. **Instale as dependências**
```bash
npm install
```

3. **Configure as variáveis de ambiente**

Crie um arquivo `.env` na pasta `be/`:
```env
GROQ_API_KEY=sua_chave_groq_aqui
ANTHROPIC_API_KEY=sua_chave_anthropic_aqui
```

4. **Execute o projeto**
```bash
# Desenvolvimento (backend + frontend)
npm run dev

# Ou execute separadamente:
npm run dev:backend  # Backend na porta 3000
npm run dev:frontend # Frontend na porta 5173
```

### URLs de Acesso

- **Frontend**: http://localhost:5173
- **Backend API**: http://localhost:3000
- **Health Check**: http://localhost:3000/health

## 🎯 Como Usar

1. **Acesse a aplicação** em http://localhost:5173
2. **Digite um prompt** descrevendo o que você quer criar:
   - "Generate a landing page for your memecoin"
   - "Build a Solana portfolio tracker using free APIs"
   - "Build a site showing crypto related news"
3. **Aguarde a geração** do código
4. **Explore os arquivos** gerados no File Explorer
5. **Visualize o resultado** na aba Preview
6. **Continue conversando** com a IA para melhorias

## 🏗️ Arquitetura

```
nexora-codedock/
├── be/                 # Backend (Node.js + Express)
│   ├── src/
│   │   ├── index.ts    # Servidor principal
│   │   ├── prompts.ts  # Sistema de prompts
│   │   └── defaults/   # Templates padrão
│   └── package.json
├── frontend/           # Frontend (React + Vite)
│   ├── src/
│   │   ├── components/ # Componentes React
│   │   ├── pages/      # Páginas da aplicação
│   │   └── hooks/      # Custom hooks
│   └── package.json
└── package.json        # Scripts principais
```

## 🔧 Scripts Disponíveis

- `npm run dev` - Executa backend + frontend em desenvolvimento
- `npm run build` - Build de produção
- `npm run start` - Executa versão de produção
- `npm run dev:backend` - Apenas backend
- `npm run dev:frontend` - Apenas frontend

## 🌐 Deploy

### Backend
- Configurado para deploy no Render
- Variáveis de ambiente necessárias: `GROQ_API_KEY`, `ANTHROPIC_API_KEY`

### Frontend
- Configurado para deploy no Vercel
- Headers CORS configurados no `vercel.json`

## 🤝 Contribuição

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 🆘 Suporte

Se você encontrar algum problema ou tiver dúvidas:

1. Verifique se todas as dependências estão instaladas
2. Confirme se as variáveis de ambiente estão configuradas
3. Verifique se as portas 3000 e 5173 estão disponíveis
4. Abra uma issue no repositório

---

**Desenvolvido com ❤️ usando IA e tecnologias modernas**