# 🎬 Gerenciador de Filmes Favoritos

Este projeto é uma aplicação web interativa desenvolvida por **Maxine Lourenço da Silva** para a matéria de **Programação Web Back-End**. 

O sistema consiste em um gerenciador de filmes (CRUD), onde o usuário pode organizar sua própria lista de filmes favoritos, realizando cadastros, edições, exclusões e buscas de forma dinâmica e intuitiva. 

## ✨ Funcionalidades

- **Cadastrar Filmes:** Adicione novos filmes à sua lista informando Título, Gênero, Ano de lançamento e uma Nota (de 0 a 10).
- **Editar Filmes:** Atualize informações e corrija dados de filmes já cadastrados de forma simples.
- **Excluir Filmes:** Remova filmes da sua lista com apenas um clique.
- **Pesquisa Dinâmica:** Busque rapidamente por filmes específicos pelo nome através de uma barra de pesquisa em tempo real.
- **Destaque de Avaliação:** Sistema de selos automáticos baseados na nota:
  - `⭐ Filme Recomendado` para filmes com nota igual ou superior a 8.
  - `📌 Filme Comum` para filmes com nota inferior a 8.
- **Efeitos Visuais:** Cards interativos que ganham destaque (`hover`) ao passar o mouse.

## 🚀 Tecnologias Utilizadas

O projeto foi construído com as seguintes ferramentas:

- **React:** Biblioteca JavaScript principal (utilizando Hooks como `useState` e `useEffect`).
- **Vite:** Ferramenta de build de alta performance para o ambiente de desenvolvimento.
- **JavaScript (ES6+) / JSX:** Lógica e estruturação das views.
- **CSS3 & CSS Modules:** Estilização responsiva e isolada por componente (`CardFilme.module.css`, `FormFilme.module.css`), evitando conflito de classes.

## 📂 Estrutura do Projeto

A aplicação foi componentizada para facilitar a manutenção e escalabilidade:

- `App.jsx`: Componente raiz que gerencia o estado global (lista de filmes, modo de edição e filtros de pesquisa).
- `FormFilme.jsx`: Componente de formulário reaproveitável, utilizado tanto para criar novos filmes quanto para salvar edições.
- `ListaFilmes.jsx`: Renderiza a grade contendo todos os filmes (ou exibe a mensagem "Nenhum filme cadastrado").
- `CardFilme.jsx`: Representa o card individual de cada filme com suas informações e botões de ação (✏️ e 🗑️).
