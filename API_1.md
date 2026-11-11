# API 1 - Os Python On

<p align="center">
  <strong>1º Semestre • 2024-2</strong><br>
  Site educativo sobre a metodologia ágil Scrum, com módulos de conteúdo e questionários interativos<br>
  Papel exercido no Scrum: <strong>Desenvolvedor</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projeto%20Acad%C3%AAmico-Fatec%20SJC-blue?style=for-the-badge" alt="Projeto Acadêmico Fatec SJC">
  <img src="https://img.shields.io/badge/Tipo-Web-informational?style=for-the-badge" alt="Aplicação web">
  <img src="https://img.shields.io/badge/Papel-Desenvolvedor-orange?style=for-the-badge" alt="Desenvolvedor">
  <img src="https://img.shields.io/badge/Status-Conclu%C3%ADdo-success?style=for-the-badge" alt="Projeto concluído">
</p>

---

<a id="atalhos"></a>

<br>

## 📌 Atalhos

- [Identificação do projeto](#identificacao-do-projeto)
- [🏢 Empresa parceira](#empresa-parceira)
- [❗ Problema](#problema)
- [✅ Solução](#solucao)
- [📅 Cronograma e entregas](#cronograma-e-entregas)
- [🔗 Link do repositório Git](#link-do-repositorio-git)
- [🖥️ Preview da aplicação](#preview-da-aplicacao)
- [🛠️ Tecnologias utilizadas](#tecnologias-utilizadas)
- [👨‍💻 Contribuições pessoais](#contribuicoes-pessoais)
- [🧠 Hard skills](#hard-skills)
- [🤝 Soft skills](#soft-skills)
- [📚 Aprendizados](#aprendizados)

---

<a id="identificacao-do-projeto"></a>

<br>

## Identificação do projeto

| Item | Descrição |
|---|---|
| Semestre do curso | 1º semestre |
| Ano e semestre | 2024-2 |
| Nome do projeto | Os Python On |
| Tipo de sistema | Site educativo (aplicação web) |
| Papel no Scrum | Desenvolvedor (Team Member) |
| Atuação técnica | Frontend e conteúdo: páginas de módulo, questionários e estilização |
| Equipe | Os Python On |
| Metodologia | Scrum, com três sprints, reviews ao fim de cada sprint e backlog com user stories |
| Situação do projeto | Concluído, incluindo as três sprints e a apresentação na Feira de Soluções |

---

<a id="empresa-parceira"></a>

<br>

## 🏢 Empresa parceira

| Item | Descrição |
|---|---|
| Cliente | Prof. Antônio Egydio |
| Contexto do desafio | Ensino da metodologia ágil Scrum para o público interno e externo da Fatec |
| Professor P2 | [Nome do professor] |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |

---

<a id="problema"></a>

<br>

## ❗ Problema

O cliente queria um material acessível para apresentar a metodologia ágil Scrum e seus artefatos ao público interno e externo da Fatec. Cada conceito deveria vir acompanhado de fundamentos, referências e exemplos práticos, para que o conteúdo não ficasse apenas na teoria.

Além do conteúdo, o site precisava oferecer formas de o visitante verificar o próprio entendimento, por meio de avaliações parciais e finais sobre os temas estudados.

---

<a id="solucao"></a>

<br>

## ✅ Solução

Desenvolvemos um **site educativo sobre Scrum**, organizado em uma página introdutória, cinco módulos de conteúdo e cinco questionários, um para cada módulo. O visitante estuda o conteúdo e, em seguida, responde perguntas de múltipla escolha com retorno imediato de acerto ou erro.

O projeto começou como um site estático em HTML, CSS e JavaScript e, na Sprint 3, foi migrado para uma aplicação **Flask**, que renderiza as páginas com templates. Na mesma sprint, o site foi publicado na **AWS** e ajustado para funcionar bem em telas de celular.

### Principais funcionalidades

- Página inicial e página de conceito, com introdução à agilidade e ao Scrum.
- Módulo 1: introdução ao Scrum, pilares e papéis.
- Módulo 2: eventos do Scrum.
- Módulo 3: auto-organização, cross-funcionalidade, gráfico Burndown, time-boxing e iteração.
- Módulo 4: Scrum comparado a outras metodologias ágeis e estudos de caso.
- Módulo 5: ferramentas de gestão, como Jira e Trello, e Scrum na transformação digital.
- Cinco questionários com cinco perguntas cada, destaque da resposta certa e da errada, placar final e opção de reiniciar.
- FAQ, menu suspenso, menu mobile e layout responsivo.

### Organização da solução

| Componente | Responsabilidade |
|---|---|
| `app.py` | Aplicação Flask com as rotas da página inicial, do conceito, dos módulos e dos questionários |
| `templates/` | Páginas HTML renderizadas com Jinja |
| `static/style.css` | Estilização única do site, incluindo a responsividade |
| `static/js/` | Lógica dos questionários, do FAQ e dos menus |
| `static/images/` | Imagens e logotipos usados no conteúdo |

---

<a id="cronograma-e-entregas"></a>

<br>

## 📅 Cronograma e entregas

| Etapa | Período | Principais entregas | Situação |
|---|---|---|---|
| Kick-off | 26/08/2024 a 06/09/2024 | Apresentação do desafio e alinhamento inicial com o cliente | Concluído |
| Sprint 1 — Concepção | 09/09/2024 a 29/09/2024 | Backlog, protótipo no Figma, primeiros conteúdos sobre Ágil, Scrum e papéis, e página inicial | Concluída |
| Sprint 2 — Desenvolvimento | 07/10/2024 a 27/10/2024 | Conteúdos sobre pilares, eventos, DoD/DoR, burndown, outras metodologias e ferramentas, além dos questionários | Concluída |
| Sprint 3 — Implementação | 04/11/2024 a 24/11/2024 | Migração para Flask, deploy na AWS, responsividade e correções | Concluída |
| Feira de Soluções | 12/12/2024 | Apresentação do projeto e demonstração da solução desenvolvida | Concluída |

---

<a id="link-do-repositorio-git"></a>

<br>

## 🔗 Link do repositório Git

- [Repositório do projeto Os Python On](https://github.com/Os-Python-On/API-OsPythonOn)

---

<a id="preview-da-aplicacao"></a>

<br>

## 🖥️ Preview da aplicação

[▶️ Assistir à demonstração completa](https://youtu.be/m6xBKumPmh0)

A demonstração percorre a página inicial, os módulos de conteúdo e os questionários, mostrando o retorno de acertos e erros e o placar ao final de cada teste.

---

<a id="tecnologias-utilizadas"></a>

<br>

## 🛠️ Tecnologias utilizadas

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" width="48" height="48" alt="Python" title="Python">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/flask/flask-original.svg" width="48" height="48" alt="Flask" title="Flask">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" width="48" height="48" alt="HTML5" title="HTML5">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" width="48" height="48" alt="CSS3" title="CSS3">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" width="48" height="48" alt="JavaScript" title="JavaScript">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/figma/figma-original.svg" width="48" height="48" alt="Figma" title="Figma">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/jira/jira-original.svg" width="48" height="48" alt="Jira" title="Jira">
</p>

| Área | Tecnologias | Aplicação no projeto |
|---|---|---|
| Backend | Python, Flask e Jinja2 | Rotas e renderização das páginas do site |
| Frontend | HTML5, CSS3 e JavaScript | Estrutura das páginas, estilização, responsividade e lógica dos questionários |
| Gráficos e ícones | Chart.js e Remixicon | Gráfico Burndown interativo e ícones da interface |
| Prototipação | Figma | Protótipo das telas na Sprint 1 |
| Implantação | AWS | Publicação do site na Sprint 3 |
| Gestão e colaboração | Jira, Git e GitHub | Backlog, acompanhamento das sprints e versionamento |

---

<a id="contribuicoes-pessoais"></a>

<br>

## 👨‍💻 Contribuições pessoais

Atuei como **desenvolvedor** no time, com foco nas páginas de conteúdo e nos questionários do site.

Na Sprint 2, fiquei responsável pelos **questionários dos módulos 2 a 5**. A partir da lógica de quiz criada por outro integrante para o Módulo 1, construí as páginas e os scripts de cada teste e escrevi suas perguntas, num total de 20 questões sobre DoD, DoR, time-boxing, incremento, Burndown, comparação entre Scrum, Kanban e XP, casos como Spotify e Microsoft e ferramentas como Jira e Trello. Também revisei e ampliei as perguntas do questionário do Módulo 1.

Na Sprint 3, desenvolvi a página do **Módulo 3**, com os textos sobre auto-organização e cross-funcionalidade, os cards de time-boxing e iteração e um **gráfico Burndown interativo com Chart.js**, que compara a linha ideal com o progresso real de uma sprint. Também escrevi a estilização dessa página, incluindo o ajuste para telas menores.

Esses questionários e a página do Módulo 3 foram mantidos na versão final do site, depois da migração para Flask.

---

<a id="hard-skills"></a>

<br>

## 🧠 Hard skills

<details>
  <summary><strong>Clique para visualizar as hard skills desenvolvidas no projeto</strong></summary>

<br>

| Hard skill | Nível de proficiência | Evidência no projeto |
|---|---|---|
| HTML5 | Sei fazer com autonomia | Criação das páginas dos questionários e do Módulo 3 |
| CSS3 | Sei fazer com autonomia | Estilização do Módulo 3, cards e media query para telas menores |
| JavaScript | Faço com ajuda | Adaptação da lógica dos questionários para os módulos 2 a 5 |
| Chart.js | Faço com ajuda | Gráfico Burndown interativo do Módulo 3 |
| Scrum | Sei fazer com autonomia | Participação nas sprints e produção de conteúdo sobre a metodologia |
| Git e GitHub | Faço com ajuda | Envio das páginas e scripts para o repositório da equipe |

</details>

---

<a id="soft-skills"></a>

<br>

## 🤝 Soft skills

<details>
  <summary><strong>Clique para visualizar as soft skills desenvolvidas no projeto</strong></summary>

<br>

| Soft skill | Exemplo pontual no projeto |
|---|---|
| Colaboração | Reaproveitei a lógica de quiz criada por um colega para manter os cinco questionários consistentes |
| Comunicação | Transformei conceitos de Scrum em perguntas e textos claros para quem está começando |
| Organização | Entreguei um questionário por módulo, acompanhando o conteúdo produzido pela equipe |
| Aprendizado contínuo | Estudei a metodologia ágil ao mesmo tempo em que a aplicava no próprio projeto |

</details>

---

<a id="aprendizados"></a>

<br>

## 📚 Aprendizados

O primeiro API foi meu primeiro contato com desenvolvimento em equipe usando Scrum. Produzir conteúdo sobre a metodologia enquanto o time a aplicava ajudou a entender, na prática, o papel de cada evento, do backlog e das reviews ao fim de cada sprint.

Do ponto de vista técnico, consolidei a base de HTML, CSS e JavaScript e tive meu primeiro contato com bibliotecas externas, como o Chart.js. Também acompanhei a migração do site estático para Flask, o que mostrou como um projeto pode evoluir de estrutura sem perder o que já foi construído.

Por fim, aprendi a importância de reaproveitar o trabalho dos colegas e de manter um padrão comum, para que partes feitas por pessoas diferentes formem um produto coerente.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | — | [➡️ API 2 • DeepCode](./API_2.md) |

</div>
