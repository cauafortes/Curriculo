# Currículo de Cauã Fortes Vieira

Este repositório contém o código HTML, CSS e JavaScript para a página de currículo online de **Cauã Fortes Vieira**. A página foi desenvolvida para apresentar informações profissionais e acadêmicas de forma clara e responsiva, sendo compatível com diferentes dispositivos, desde desktops até smartphones.

## Estrutura do Projeto

O projeto está dividido em dois principais arquivos:

- **index.html**: Contém o conteúdo HTML do currículo, incluindo seções como informações pessoais, resumo profissional, formação acadêmica, experiência profissional e habilidades.
- **styles.css**: Arquivo de estilo que define o design e layout da página, tornando-a visualmente agradável e responsiva.
  
## Funcionalidades

### Navegação
A página inclui uma barra de navegação fixa no topo, que permite fácil acesso às principais seções do currículo, como:
- Informações Pessoais
- Resumo Profissional
- Formação Acadêmica
- Experiência Profissional
- Habilidades
- Contato

### Seções Colapsáveis
Cada seção principal da página (como Informações Pessoais, Resumo Profissional etc.) pode ser expandida ou recolhida com um clique no título da seção. Isso permite uma navegação mais organizada e fácil para o usuário.

### Área Lateral (Aside)
Uma área lateral foi adicionada com informações complementares, como:
- **Projetos Acadêmicos**:
  - Sistema Mercado Nova Machado (C# e SQL)
  - Jungle Game (Godot e GDScript)
- **Interesses**:
  - Desenvolvimento de Software
  - Inteligência Artificial
  - Segurança de Redes

Essa área fornece uma visão rápida sobre os projetos e interesses do autor.

### Responsividade
O layout da página foi projetado para ser responsivo, adaptando-se a diferentes tamanhos de tela:
- Em telas maiores (desktops), o conteúdo principal (`main`) e a área lateral (`aside`) são exibidos lado a lado.
- Em telas menores (smartphones), o layout se ajusta automaticamente para empilhar o conteúdo, exibindo o `aside` abaixo do conteúdo principal.

## Scripts
A página utiliza JavaScript simples para controlar o comportamento das seções colapsáveis, permitindo expandir e recolher o conteúdo ao clicar no título de cada seção.

```javascript
const sections = document.querySelectorAll('.collapsible-section h2');
sections.forEach(section => {
    section.addEventListener('click', () => {
        section.nextElementSibling.classList.toggle('active');
    });
});
