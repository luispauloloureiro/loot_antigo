# 🏺 Loot Antigo | Câmara das Relíquias

**Versão 1.29.04** • Marketplace gamificado de artefatos épicos

![Loot Antigo Banner](https://via.placeholder.com/1200x400/1E140A/D4AF37?text=LOOT+ANTIGO+-+CÂMARA+DAS+RELÍQUIAS)

> Uma experiência imersiva de marketplace RPG com autenticação completa, sistema de postagem de itens e design premium inspirado em jogos AAA.

---

## ✨ Sobre o Projeto

**Loot Antigo** é um marketplace digital temático de RPG onde aventureiros podem comprar, vender e colecionar relíquias lendárias. 

O projeto combina **design cinematográfico**, **mecânicas gamificadas** e **tecnologia moderna** para entregar uma experiência única, ideal para demonstração de portfólio de alto nível.

### Versão Atual: **1.29.04**

---

## 🎮 Funcionalidades Principais

### ✅ Implementadas
- **Autenticação Completa** com Firebase
  - Login e cadastro com Email/Senha
  - Login com Google
  - Recuperação de senha
  - Verificação de email automática
  - Indicador de força de senha em tempo real

- **Sistema de Postagem de Itens** (Wizard Multi-step)
- **Dashboard Imersiva** com filtros avançados (classe, raridade, preço, ordenação)
- **Carrinho Persistente** com controle de estoque
- **Área "Meus Artefatos"** (itens postados pelo usuário)
- **Backend Customizado (NOVO)** com Node.js, Express e MongoDB
- **Upload de Imagens Local** gerenciado através do Multer
- **Design Temático Premium** com glassmorphism e micro-interações
- **Totalmente Responsivo** (Mobile First)

### 🔜 Em Desenvolvimento
- Avaliações e favoritos
- Chat entre comprador e vendedor
- Perfil do usuário editável

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia          | Versão    | Propósito                     |
|---------------------|-----------|-------------------------------|
| **React.js**        | 18.3      | Biblioteca principal          |
| **Node.js**         | 18+       | Runtime do Backend e API      |
| **Express**         | 4.x       | Framework Web                 |
| **MongoDB**         | -         | Banco de Dados (Mongoose)     |
| **Tailwind CSS**    | 3.4       | Estilização                   |
| **Firebase**        | 9.23      | Apenas Autenticação de Usuário|
| **React Context**   | -         | Gerenciamento de estado       |

**Outras ferramentas:**
- Multer, Cors, Dotenv, Mongoose, Vite

---

## 🚀 Como Executar Localmente

### Pré-requisitos
- Node.js (v18 ou superior)
- MongoDB rodando localmente na porta 27017 (ou URI do Atlas)
- Conta no [Firebase](https://console.firebase.google.com/)

### Passo a passo

```bash
# 1. Clone o repositório
git clone https://github.com/luipauloloureiro/loot_antigo.git
cd loot_antigo

# 2. Instale as dependências
npm install

# 3. Configure as variáveis de ambiente
cp .env.example .env
# Adicione no .env a variável MONGO_URI (ex: mongodb://127.0.0.1:27017/loot_antiqua) e credenciais do Firebase

# 4. Inicie o Servidor Backend (API e Servidor de Imagens)
node server.js

# 5. Em outro terminal, inicie o Frontend
npm run dev
```

---

## 📈 Melhorias Futuras

### Funcionalidades
- Sistema de favoritos
- Histórico de compras
- Avaliações e comentários
- Chat entre comprador/vendedor
- Notificações (novos itens, vendas)
- Dashboard de vendas (gráficos)

### Técnicas
- Testes (Jest + React Testing Library)
- CI/CD (GitHub Actions)
- Typescript
- PWA (service workers)
- Infinite scroll
- Debounce em buscas

### UX
- Dark mode
- Animações mais elaboradas (Framer Motion)
- Skeleton loaders
- Toasts melhores (react-hot-toast)
- Tutorial inicial (onboarding)

---

## 🎯 Nota Final: 7.5/10

**Pontos Positivos:**
- Design único e criativo ✨
- Código organizado e legível
- Autenticação robusta
- UX gamificada engajante

**Pontos a Melhorar:**
- Backend real (crítico para produção)
- Segurança (variáveis de ambiente)
- Gestão de estado centralizada
- Validações completas

---

## 🚀 Próximos Passos Sugeridos

**Curto Prazo (1-2 semanas)**
- Implementar Firebase Firestore
- Configurar Firebase Storage
- Adicionar validações de formulário
- Mover credenciais para `.env`

**Médio Prazo (1 mês)**
- Criar `ProductsContext`
- Implementar testes básicos
- Adicionar loading states consistentes
- Melhorar acessibilidade

**Longo Prazo (2-3 meses)**
- Sistema de notificações
- Dashboard de vendas
- Chat em tempo real
- Deploy com CI/CD