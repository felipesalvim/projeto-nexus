# Website Institucional - Nexus Innova

\<p align="center"\>
\<img src="/images/captura-site.png" alt="Banner do Projeto Nexus Innova" width="1000"/\>
\</p\>

## 📋 Índice

  - [🎯 Sobre o Projeto]
  - [🚀 Tecnologias Utilizadas]
  - [📁 Estrutura do Projeto]
  - [⚡ Funcionalidades]
  - [🏗️ Arquitetura e Padrões]
  - [🛠️ Instalação e Configuração]
  - [💻 Uso]
  - [🔍 SEO e Performance]
  - [♿ Acessibilidade]
  - [🔒 Segurança]
  - [🤝 Contribuindo]
  - [📄 Licença]
  - [📞 Contato]

## 🎯 Sobre o Projeto

O **"Nexus Innova"** é um website institucional desenvolvido para uma empresa júnior de tecnologia da informação. O projeto foi construído com **HTML5**, **CSS3** e **JavaScript puro (Vanilla JS)**, seguindo princípios modernos de desenvolvimento web, com foco em performance, acessibilidade и experiência do usuário.

### Objetivos

  * Apresentar os "serviços" da empresa de forma clara e profissional
  * Criar um "portfólio interativo" de projetos
  * Estabelecer um "canal de comunicação" eficiente com potenciais clientes
  * Compartilhar conhecimento através de um "blog técnico"
  * Demonstrar expertise em "desenvolvimento web"

## 🚀 Tecnologias Utilizadas

### Frontend

  * **HTML5**: Estrutura "semântica" e acessível
  * **CSS3**: Estilização moderna com "variáveis CSS", "Grid" e "Flexbox"
  * **JavaScript (ES6+)**: Lógica de aplicação "sem frameworks"
  * **AOS (Animate On Scroll)**: Animações suaves durante o scroll
  * **Font Awesome**: Biblioteca de ícones

### Backend

  * **PHP 7.4+**: Processamento de formulários
  * **MySQL**: Armazenamento de dados de contato

### Ferramentas e Bibliotecas

  * **Google Fonts (Poppins)**: Tipografia moderna
  * **CDN Cloudflare**: Distribuição de bibliotecas externas
  * **Schema.org**: Dados estruturados para SEO

## 📁 Estrutura do Projeto

```
nexus-innova/
│
├── index.html              # Página principal
├── blog.html               # Listagem de posts do blog
├── style.css               # Estilos globais
├── script.js               # Lógica principal da aplicação
├── data.js                 # Dados centralizados (conteúdo dinâmico)
├── salvar_contato.php      # Backend para processamento de formulários
│
├── blog/
│   └── post.html           # Template de post individual
│
├── projetos/
│   └── projeto.html        # Template de projeto individual
│
├── images/                 # Imagens do site
│   ├── logo.png
│   ├── logo-nexus-white.png
│   ├── hero-background.png
│   ├── og-image.png
│   ├── favicon.ico
│   ├── favicon.svg
│   ├── apple-touch-icon.png
│   └── membros/            # Fotos da equipe
│
├── blog/images/            # Imagens dos posts do blog
│
├── projetos/images/        # Imagens dos projetos
│
└── documentos/             # PDFs de serviços
```

## ⚡ Funcionalidades

1.  **"Navegação Responsiva"**

      * Menu hambúrguer para dispositivos móveis
      * Navegação fluida com scroll suave
      * Header fixo com efeito de transparência ao rolar

2.  **"Seções Dinâmicas"**

      * **Hero**: Apresentação impactante com call-to-action
      * **Sobre**: Informações sobre a empresa
      * **Processo**: Metodologia de trabalho em 4 etapas
      * **Equipe**: Apresentação dos membros com links sociais
      * **Serviços**: Cards interativos com PDFs para download
      * **Projetos**: Portfólio filtrado por status e tecnologias
      * **Blog**: Artigos técnicos com busca integrada
      * **Contato**: Quiz interativo para qualificação de leads

3.  **"Sistema de Blog"**

      * Listagem de posts com busca em tempo real
      * Posts individuais com SEO otimizado
      * Breadcrumbs para navegação
      * Sistema de posts relacionados
      * Meta tags dinâmicas
      * Dados estruturados (JSON-LD)

4.  **"Portfólio de Projetos"**

      * Detalhamento completo de cada projeto
      * Formulário de contato integrado com validação
      * Status de projeto ("Concluído" / "Em Andamento")
      * Tags de tecnologias utilizadas
      * Links para demonstração ao vivo

5.  **"Quiz Interativo"**

      * Sistema de qualificação de leads por etapas
      * Histórico de navegação (botão "Voltar")
      * Redirecionamento automático para WhatsApp
      * Mensagens contextualizadas por especialista

6.  **"Chatbot Flutuante"**

      * Assistente virtual com fluxo conversacional
      * Coleta de informações do usuário (nome e email)
      * Direcionamento para especialistas via WhatsApp
      * Integração com PDFs de apresentação
      * Animações suaves de entrada/saída

7.  **"Componentes de Contato"**

      * Botão flutuante do WhatsApp com texto expansível
      * Formulários com validação client-side
      * Proteção contra "SQL Injection" no backend
      * Feedback visual de sucesso/erro

## 🏗️ Arquitetura e Padrões

### Princípios de Design

  * **"DRY (Don't Repeat Yourself)"**

      * Funções reutilizáveis para renderização de componentes
      * Dados centralizados em `data.js`
      * Template único para posts e projetos

  * **"Separation of Concerns"**

      * **HTML** para estrutura semântica
      * **CSS** para apresentação visual
      * **JavaScript** para comportamento e interatividade
      * **PHP** para lógica de servidor

  * **"Mobile-First"**

      * Design responsivo com breakpoints estratégicos
      * Navegação adaptativa
      * Imagens otimizadas com `loading="lazy"`

### Organização do Código JavaScript

```javascript
// Estrutura modular em script.js
// 1. Variáveis Globais
// 2. Funções Principais (Navegação, Injeção de Conteúdo)
// 3. Funções de Otimização (SEO, Performance)
// 4. Funções de Renderização (DRY)
// 5. Lógica de Formulários
// 6. Sistema de Quiz
// 7. Sistema de Chatbot
// 8. Event Listeners & Initialization
```

## 🛠️ Instalação e Configuração

### Pré-requisitos

  * Servidor web (Apache, Nginx, ou similar)
  * PHP 7.4 ou superior
  * MySQL 5.7 ou superior
  * Navegador moderno com suporte a ES6+

### Configuração do Banco de Dados

1.  Crie o banco de dados:
    ```sql
    CREATE DATABASE nexus_innova_db CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
    ```
2.  Crie a tabela de contatos:
    ```sql
    USE nexus_innova_db;

    CREATE TABLE contatos_projetos (
        id INT AUTO_INCREMENT PRIMARY KEY,
        nome VARCHAR(255) NOT NULL,
        telefone VARCHAR(20),
        email VARCHAR(255) NOT NULL,
        projeto_id VARCHAR(100) NOT NULL,
        data_contato TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
        INDEX idx_email (email),
        INDEX idx_projeto (projeto_id)
    ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_unicode_ci;
    ```
3.  Configure as credenciais em `salvar_contato.php`:
    ```php
    $servername = "localhost";
    $username = "seu_usuario";
    $password = "sua_senha";
    $dbname = "nexus_innova_db";
    ```

## 💻 Uso

### Adicionando Novo Post ao Blog

Edite `data.js` e adicione ao array `blogPosts`:

```javascript
{
    id: 'slug-do-post',
    title: 'Título do Post',
    description: 'Descrição breve',
    image: '/blog/images/imagem.png',
    date: 'DD de mês, YYYY',
    tags: ['Tag1', 'Tag2'],
    content: `
        <p>Conteúdo HTML do post...</p>
        <h2>Subtítulo</h2>
        <p>Mais conteúdo...</p>
    `
}
```

### Adicionando Novo Projeto

Edite `data.js` e adicione ao array `highlightedProjects`:

```javascript
{
    id: 'slug-do-projeto',
    title: 'Nome do Projeto',
    image: '/projetos/images/projeto.png',
    description: 'Descrição resumida',
    status: 'Concluído', // ou 'Em Andamento'
    technologies: ['React', 'Node.js'],
    details: {
        challenge: 'Descrição do desafio...',
        solution: 'Descrição da solução...',
        results: 'Resultados obtidos...',
        projectImage: '/projetos/images/projeto.png',
        liveUrl: 'https://projeto.com', // opcional
        githubUrl: 'https://github.com/...' // opcional
    }
}
```

## 🔍 SEO e Performance

### Otimizações Implementadas

  * **"Meta Tags Dinâmicas"**: Título, descrição, Open Graph e Twitter Cards únicos por página.
  * **"Dados Estruturados"**: Schema.org JSON-LD para posts, melhorando a indexação.
  * **"Performance"**: Lazy loading de imagens, animações com AOS, e cache eficiente de arquivos.

## ♿ Acessibilidade

  * **"HTML Semântico"**: Uso correto de tags como `<header>`, `<main>`, `<article>`.
  * **"Navegação Acessível"**: Funcionalidade via teclado e contraste de cores adequado (WCAG 2.1).
  * **"Atributos Essenciais"**: `alt` em imagens e `labels` em formulários.

## 🔒 Segurança

  * **"Backend (PHP)"**: Uso de "Prepared Statements" para proteção contra SQL Injection e sanitização de inputs.
  * **"Frontend"**: Validação de formulários no lado do cliente e proteção contra XSS.

## 🤝 Contribuindo

Contribuições são bem-vindas\! Para contribuir:

1.  **"Fork"** o projeto
2.  Crie uma **"Branch"** para sua feature (`git checkout -b feature/NovaFuncionalidade`)
3.  **"Commit"** suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`)
4.  **"Push"** para a branch (`git push origin feature/NovaFuncionalidade`)
5.  Abra um **"Pull Request"**

## 📄 Licença

Este projeto é proprietário da **"Nexus Innova"**. Todos os direitos reservados.

## 📞 Contato

**Nexus Innova**

  * **Repositório Github:** [https://github.com/felipesalvim/projeto-nexus-innova](https://github.com/felipesalvim/projeto-nexus-innova)
  * **Website:** [https://www.nexusinnova.com.br](https://www.nexusinnova.com.br)
  * **Email:** contato@nexusinnova.com.br
  * **Instagram:** @nexus_innova

-----

*Desenvolvido com 💚 pela equipe Nexus Innova*# nexus_innova
