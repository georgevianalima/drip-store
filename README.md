# 🛍️ Loja Drip - E-commerce Frontend

Um projeto de e-commerce moderno construído com **React**, **Vite** e **Tailwind CSS**. A aplicação oferece uma experiência de compra completa com autenticação de usuários, catálogo de produtos, filtros avançados, carrinho de compras e gerenciamento de pedidos.

---

## 📋 Sobre o Projeto

**Loja Drip** é uma plataforma de e-commerce especializada em roupas, calçados e acessórios. O projeto foi desenvolvido como parte do programa **Geração Tech FullStack** e implementa funcionalidades essenciais de uma loja online moderna.

### Principais Funcionalidades
- 👤 **Autenticação**: Login e cadastro de usuários
- 🛒 **Carrinho de Compras**: Adicionar, remover e gerenciar produtos
- 🔍 **Filtros Avançados**: Por categoria, marca, gênero e condição
- 📦 **Catálogo de Produtos**: Visualização detalhada de itens
- 📋 **Histórico de Pedidos**: Acompanhe seus pedidos
- 🎨 **Design Responsivo**: Layout mobile-first com Tailwind CSS
- ⚡ **Performance**: Vite com HMR para desenvolvimento rápido

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Versão | Descrição |
|-----------|--------|-----------|
| **React** | 19.2.0 | Biblioteca para construção de interfaces |
| **Vite** | 7.3.1 | Bundler e dev server ultra-rápido |
| **React Router** | 7.13.1 | Roteamento client-side |
| **Tailwind CSS** | 4.2.1 | Framework CSS utilitário |
| **Axios** | 1.13.6 | Cliente HTTP para requisições |
| **React Icons** | 5.5.0 | Ícones SVG para React |
| **ESLint** | 9.39.1 | Linter para qualidade de código |

---

## 📁 Estrutura do Projeto

``
loja-drip/
├── src/
│   ├── pages/                 # Páginas da aplicação
│   │   ├── homePage.jsx       # Página inicial
│   │   ├── productPage.jsx    # Listagem de produtos com filtros
│   │   ├── productViewPage.jsx # Detalhes do produto
│   │   ├── categoriasPage.jsx # Página de categorias
│   │   ├── login.jsx          # Tela de login
│   │   ├── cadastro.jsx       # Tela de cadastro
│   │   ├── completarCadastro.jsx # Complementar dados do cadastro
│   │   ├── meusPedidosPage.jsx    # Histórico de pedidos
│   │   └── layout.jsx         # Layout comum
│   ├── components/            # Componentes reutilizáveis
│   │   ├── header.jsx         # Cabeçalho
│   │   ├── footer.jsx         # Rodapé
│   │   ├── mainNave.jsx       # Navegação principal
│   │   ├── searchBar.jsx      # Barra de busca
│   │   ├── productInfo.jsx    # Informações do produto
│   │   ├── gallery.jsx        # Galeria de imagens
│   │   ├── cartIcon.jsx       # Ícone do carrinho
│   │   ├── cartDropDown.jsx   # Menu suspenso do carrinho
│   │   ├── filterGroup.jsx    # Grupo de filtros
│   │   ├── logo.jsx           # Logo da marca
│   │   ├── authLinks.jsx      # Links de autenticação
│   │   ├── buyBox.jsx         # Caixa de compra
│   │   ├── relatedProducts.jsx # Produtos relacionados
│   │   ├── section.jsx        # Componente de seção genérico
│   │   ├── AbaProdutos/       # Componentes de listagem
│   │   │   ├── productCardList.jsx
│   │   │   └── productListingList.jsx
│   │   └── HomePage/          # Componentes da página inicial
│   │       ├── productCard.jsx
│   │       └── productListing.jsx
│   ├── contexts/              # Context API
│   │   └── cartContext.jsx    # Contexto do carrinho
│   ├── services/              # Serviços (API, etc)
│   │   └── api.js             # Configuração do Axios
│   ├── data/                  # Dados estáticos
│   │   └── products.js        # Catálogo de produtos
│   ├── assets/                # Imagens e recursos
│   ├── App.jsx                # Componente raiz
│   ├── index.css              # Estilos globais
│   └── main.jsx               # Entrada da aplicação
├── public/                    # Arquivos públicos
├── vite.config.js             # Configuração do Vite
├── tailwind.config.js         # Configuração do Tailwind
├── postcss.config.js          # Configuração do PostCSS
├── eslint.config.js           # Configuração do ESLint
├── package.json               # Dependências do projeto
└── README.md                  # Este arquivo
``

---

## 🚀 Como Instalar e Rodar

### Pré-requisitos
- **Node.js** versão 16+ instalado
- **npm** ou **yarn** para gerenciamento de pacotes

### Instalação

1. **Clone o repositório** (se aplicável)
   \\\ash
   git clone <url-do-repositorio>
   cd loja-drip
   \\\

2. **Instale as dependências**
   \\\ash
   npm install
   \\\

3. **Configure as variáveis de ambiente** (se necessário)
   - Crie um arquivo \.env.local\ na raiz do projeto
   - Configure a URL da API (exemplo): \VITE_API_URL=http://localhost:3000\

### Executar em Desenvolvimento

\\\ash
npm run dev
\\\

A aplicação abrirá em \http://localhost:5173\ com **Hot Module Replacement (HMR)** ativado. Qualquer mudança será refletida automaticamente no navegador.

### Build para Produção

\\\ash
npm run build
\\\

Gera os arquivos otimizados na pasta \dist/\.

### Preview do Build

\\\ash
npm run preview
\\\

Visualiza a versão de produção localmente.

### Verificar Qualidade do Código

\\\ash
npm run lint
\\\

Executa o ESLint para verificar a qualidade do código.

---

## 📚 Scripts Disponíveis

| Script | Descrição |
|--------|-----------|
| \
pm run dev\ | Inicia o servidor de desenvolvimento |
| \
pm run build\ | Constrói a aplicação para produção |
| \
pm run preview\ | Visualiza o build de produção |
| \
pm run lint\ | Executa validação de código com ESLint |

---

## 🎯 Funcionalidades Detalhadas

### 1. **Autenticação**
- Registro de novos usuários com validação
- Login com credenciais
- Complementação de dados do cadastro
- Gerenciamento de sessão

### 2. **Catálogo de Produtos**
- Listagem de todos os produtos
- Visualização detalhada de cada produto
- Galeria de imagens
- Informações de preço, categoria, marca e condição

### 3. **Sistema de Filtros**
- Filtro por **Marca**: Adidas, Nike, Puma, Balenciaga, etc.
- Filtro por **Categoria**: Camisetas, Calças, Bonés, Headphones, Tênis
- Filtro por **Gênero**: Masculino, Feminino, Unisex
- Filtro por **Condição**: Novo, Usado
- Busca por texto livre
- Ordenação por preço (menor → maior, maior → menor)

### 4. **Carrinho de Compras**
- Adicionar/remover produtos
- Visualização rápida via dropdown
- Cálculo automático do total
- Persistência de dados (Context API)

### 5. **Pedidos**
- Visualização de histórico de pedidos
- Acompanhamento de status
- Detalhes de cada pedido

---

## 🗂️ Componentes Principais

### \Pages\
- **homePage.jsx**: Landing page com featured products
- **productPage.jsx**: Catálogo com filtros avançados e ordenação
- **productViewPage.jsx**: Detalhes completos de um produto
- **login.jsx** / **cadastro.jsx**: Autenticação de usuários
- **meusPedidosPage.jsx**: Dashboard de pedidos do usuário

### \Components\
- **header.jsx**: Cabeçalho com navegação e carrinho
- **filterGroup.jsx**: Componente reutilizável de filtros
- **productCard.jsx**: Card individual de produto
- **cartDropDown.jsx**: Menu suspenso do carrinho

### \Contexts\
- **cartContext.jsx**: Gerenciamento global do estado do carrinho

### \Services\
- **api.js**: Configuração centralizada do Axios para requisições HTTP

---

## 🎨 Customização com Tailwind CSS

O projeto usa **Tailwind CSS 4.2.1** com a compilação via Vite. Principais configurações:

- **Tema personalizado** em \	ailwind.config.js\
- **Cores principais**: Rosa (\pink-500\, \pink-700\), Cinza (\gray-*\)
- **Plugins Tailwind**: Forms, Typography
- **Utilitários responsivos**: \sm:\, \md:\, \lg:\ prefixes

Para adicionar novos estilos, edite as classes direto no JSX ou estenda \	ailwind.config.js\.

---

## 🔌 Integração com API

A aplicação comunica-se com um backend via **Axios**. Exemplo de configuração em \services/api.js\:

\\\javascript
import axios from 'axios';

const api = axios.create({
  baseURL: process.env.VITE_API_URL || 'http://localhost:3000/api',
});

export default api;
\\\

**Endpoints esperados** (exemplo):
- \GET /products\ - Listar produtos
- \POST /auth/login\ - Autenticação
- \POST /auth/register\ - Registro
- \GET /orders\ - Listar pedidos do usuário

---

## 📱 Responsividade

O projeto foi construído com a abordagem **mobile-first**:
- **Mobile**: 100% da largura
- **Tablet** (\md:\): Layouts adaptados
- **Desktop** (\lg:\): Layout completo com sidebar de filtros

---

## 🐛 Troubleshooting

### Erro: "Cannot find module"
\\\ash
npm install
\\\

### HMR não funciona
Verifique a URL em \ite.config.js\ e as configurações de rede.

### Estilos Tailwind não aparecem
Certifique-se de que a configuração do Tailwind está correta e que o servidor de desenvolvimento está rodando.

### Requisições à API falham
Verifique:
- Se a API está rodando
- Se a URL base em \VITE_API_URL\ está correta
- Configurações de CORS no backend

---

## 📝 Licença

Este projeto foi desenvolvido como parte do programa **Geração Tech FullStack**.

---

## 👥 Contribuindo

Para contribuir com o projeto:

1. Crie uma branch para sua feature (\git checkout -b feature/nova-funcionalidade\)
2. Commit suas mudanças (\git commit -m 'Adiciona nova funcionalidade'\)
3. Push para a branch (\git push origin feature/nova-funcionalidade\)
4. Abra um Pull Request

---

## 📧 Suporte

Para dúvidas ou problemas, abra uma **issue** no repositório.

---

**Última atualização**: Março 2026 | **Versão**: 0.0.0
