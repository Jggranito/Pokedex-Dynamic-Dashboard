# ⚡ Pokedex Dynamic Dashboard

![Project Banner](./src/screenshot/preview.png)
> *Nota: Substitua `./src/screenshot/preview.png` pelo caminho da sua imagem principal.*

**Uma Single Page Application (SPA) robusta para consulta e análise de dados da PokeAPI. Focada em performance, arquitetura de componentes e experiência do usuário (UX).**

## 📖 Sobre o Projeto
Este projeto vai além de uma simples lista de Pokémons. Trata-se de uma aplicação completa de consumo de API RESTful que gerencia grandes volumes de dados aninhados (nested data). 

O objetivo foi criar uma interface moderna e responsiva onde o usuário pode não apenas buscar, mas analisar profundamente os atributos, movimentos e estatísticas de cada Pokémon, alternando entre temas visuais (Dark/Light Mode) sem recarregar a página.

## 🚀 Funcionalidades Principais

### 🔍 Busca e Filtragem Avançada
- **Search Engine:** Pesquisa em tempo real por Nome ou ID.
- **Filtros Dinâmicos:** Seleção por Tipagem (Fire, Water, etc.) afetando a listagem imediatamente.
- **Paginação Otimizada:** Sistema de "Load More" para carregar dados sob demanda, economizando banda e processamento.

### 📊 Análise Detalhada (Dashboard)
Ao selecionar um Pokémon, o usuário acessa um painel com 3 abas de dados:
1.  **Geral:** Dados vitais, XP base e tipagem.
2.  **Status (Base Stats):** Gráficos visuais de HP, Attack, Defense, Speed, etc.
3.  **Moveset Inteligente:** Lista completa de golpes filtrada por método de aprendizado (Level Up, TMs, Egg Moves, Tutor).
    * *Detalhe:* Ao clicar em um golpe, um modal exibe Power, Accuracy, PP e a descrição técnica do movimento.

### 🎨 UI/UX & Customização
- **Theme Switcher:** Alternância global entre **Dark Mode** e **Light Mode** utilizando Context API para persistência de estado.
- **Layout Responsivo:** Adaptação fluida para Mobile, Tablet e Desktop.

## 🛠️ Tecnologias & Arquitetura

O projeto foi construído seguindo os princípios do **Clean Code** e Componentização.

| Tech | Função no Projeto |
| :--- | :--- |
| **React.js** | Biblioteca core para construção da interface declarativa. |
| **Context API** | Gerenciamento de estado global (Temas e Dados do Usuário). |
| **Styled Components** | Estilização CSS-in-JS dinâmica e escopada. |
| **React Router DOM** | Roteamento client-side para navegação fluida (SPA). |
| **Axios / Fetch** | Camada de serviço para consumo da PokeAPI. |

## 💡 Desafios Técnicos Superados

1.  **Drilling de Propriedades:** O uso da Context API eliminou a necessidade de passar props de tema manualmente por dezenas de componentes.
2.  **Complexidade da API:** A PokeAPI possui dados extremamente aninhados. Foi criada uma camada de tratamento de dados para "limpar" o JSON antes de renderizar na tela, garantindo que componentes de UI recebam apenas o necessário.
3.  **Performance de Renderização:** Otimização do carregamento de imagens e listas longas para evitar engasgos na rolagem.

## 🔗 Links

- **Repositório:** [Acesse o Código](https://github.com/Jggranito/Pokedex-Dynamic-Dashboard)
- **Live Preview:** [Ver Projeto Online](https://jggranito.github.io/Pokedex-Dynamic-Dashboard/)

---

Desenvolvido por **[João Gabriel Granito](https://www.linkedin.com/in/jo%C3%A3o-gabriel-granito-77666a262/)**
*Mobile Developer & Front-End Specialist*
