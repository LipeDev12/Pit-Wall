# 🏎️ Pit Wall — Landing Page F1 (GP de São Paulo)

Bem-vindo ao repositório do projeto **Pit Wall**, uma *landing page* temática e responsiva sobre a Formula 1 e o Grande Prêmio de São Paulo em Interlagos. 

Este projeto foi desenvolvido como atividade prática e de estudo de **HTML5** e **CSS3** no curso de **Tecnologia da Informação (TI) do SENAI**, sob orientação do **Professor Denani**.

---

## 📌 Sumário

- [Visão Geral](#-visão-geral)
- [Funcionalidades e Seções](#-funcionalidades-e-seções)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Destaques do CSS](#-destaques-do-css)
- [Como Executar](#-como-executar)
- [Autoria e Créditos](#-autoria-e-créditos)

---

## 🏎️ Visão Geral

O **Pit Wall** é uma interface moderna e imersiva inspirada na identidade visual oficial da Fórmula 1 e do ecossistema F1 TV. A aplicação apresenta informações sobre o GP de São Paulo, perfil e cards das equipes/pilotos, tabela interativa de classificação e um sistema de reserva e compra de ingressos.

---

## 🎯 Funcionalidades e Seções

1. **Barra de Navegação (`header.topbar`):**
   - Logo estilizada com destaque de cores.
   - Menu de navegação rápido com links internos (âncoras).
   - Botão em destaque para garantia de ingressos.

2. **Banner Principal (`section.hero`):**
   - Apresentação do GP de Interlagos com dados do circuito (voltas, extensão, número de curvas).
   - Botões com chamadas para ação (*Call to Action*).
   - Fundo dinâmico com gradiente e imagem temática da Scuderia Ferrari.

3. **Faixa Zebra / Kerb (`.kerb`):**
   - Elemento visual personalizado criado exclusivamente em CSS com `repeating-linear-gradient` para simular a zebra zebrada clássica das pistas de corrida.

4. **Grid de Pilotos (`#pilotos`):**
   - Cards dinâmicos e responsivos exibindo número do carro, piloto e equipe.
   - Temas visuais e gradientes específicos para cada equipe (Ferrari, Mercedes, Red Bull, McLaren).
   - Animação de elevação (*hover effect*) ao passar o ponteiro do mouse.

5. **Tabela de Classificação e Filtros (`#classificacao`):**
   - Formulário com campos de pesquisa por piloto e seleção por equipe.
   - Tabela estilizada estilo F1 TV com marcadores visuais das equipes, destaque especial para o líder do campeonato e rolagem horizontal em telas menores.

6. **Área de Ingressos & Formulário (`#ingressos`):**
   - Lista de preços por setor (Arquibancada A, Setor da Reta, Box VIP) e caixas de alerta.
   - Formulário completo estruturado em Grid 2 colunas com suporte a uploads de fotos da torcida, datas, inputs numéricos e envio de recados.

7. **Design Responsivo:**
   - Adaptação completa para dispositivos móveis, tablets e computadores por meio de *Media Queries*.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5:** Estruturação semântica do documento (`header`, `nav`, `main`, `section`, `form`, `footer`, etc.).
- **CSS3:**
  - Variáveis CSS (`:root`) para padronização da paleta de cores.
  - Flexbox e CSS Grid Layout para aliamento e organização responsiva dos elementos.
  - Gradientes e animações de transição suave (`transition`, `transform`).
- **Google Fonts:** Tipografia oficial *Titillium Web*.

---

## 📂 Estrutura do Projeto

```text
├── index.html        # Estrutura principal da página HTML
├── style.css         # Estilização completa, variáveis, componentes e responsividade
└── img/
    └── img/
        └── FerrariLH.jpg   # Imagem de fundo e favicon do projeto
```

---

## 🎨 Destaques do CSS

- **Variáveis Globais (`:root`):**
  Facilitam a manutenção de cores e fontes do projeto:
  - Cores base: `--black`, `--panel`, `--red`, `--white`, `--muted`, `--line`.
  - Cores das equipes: `--ferrari`, `--mclaren`, `--mercedes`, `--redbull`, `--audi`.

- **Zebras da Pista em CSS PURO:**
  ```css
  .kerb {
      height: 12px;
      width: 100%;
      background: repeating-linear-gradient(90deg,
          var(--red) 0, var(--red) 40px,
          var(--white) 40px, var(--white) 80px);
  }
  ```

---

## 🚀 Como Executar

1. Faust o clone ou faça o download dos arquivos do repositório.
2. Certifique-se de manter a estrutura de pastas e a imagem `FerrariLH.jpg` dentro do caminho `img/img/`.
3. Abra o arquivo `index.html` em qualquer navegador web moderno (Google Chrome, Microsoft Edge, Firefox, etc.).

---

## 👨‍💻 Autoria e Créditos

- **Desenvolvedor:** Gabriel Caprari Viezzer
- **Orientador:** Prof. Denani
- **Instituição:** SENAI — Curso Técnico / Qualificação em Tecnologia da Informação (TI)
- **Finalidade:** Estudo e prática de desenvolvimento Web Front-End (HTML5 e CSS3)
