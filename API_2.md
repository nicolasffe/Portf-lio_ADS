# API 2 - DeepCode

<p align="center">
  <strong>2º Semestre • 2025-1</strong><br>
  Ambiente de desenvolvimento desktop com assistente de IA local para análise e correção de código<br>
  Papel exercido no Scrum: <strong>Desenvolvedor</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projeto%20Acad%C3%AAmico-Fatec%20SJC-blue?style=for-the-badge" alt="Projeto Acadêmico Fatec SJC">
  <img src="https://img.shields.io/badge/Tipo-Desktop%20com%20IA-informational?style=for-the-badge" alt="Aplicação desktop com IA">
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
| Semestre do curso | 2º semestre |
| Ano e semestre | 2025-1 |
| Nome do projeto | DeepCode |
| Tipo de sistema | Aplicação desktop com assistente de IA local |
| Papel no Scrum | Desenvolvedor (Team Member) |
| Atuação técnica | Frontend desktop: prototipação no Figma, interface em JavaFX e estilização |
| Equipe | DeepCode |
| Metodologia | Scrum, com três sprints, reviews, backlog no Jira e gráficos de burndown |
| Situação do projeto | Concluído, incluindo as três sprints e a apresentação na Feira de Soluções |

---

<a id="empresa-parceira"></a>

<br>

## 🏢 Empresa parceira

| Item | Descrição |
|---|---|
| Cliente | Professores da Fatec São José dos Campos |
| Contexto do desafio | Apoio a desenvolvedores na análise e correção de código com inteligência artificial |
| Professor P2 | [Nome do professor] |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |

---

<a id="problema"></a>

<br>

## ❗ Problema

O desafio era desenvolver um ambiente de desenvolvimento que ajudasse o programador a otimizar seu tempo e reduzir custos, apoiando a identificação e a correção de erros no código. Também se esperava que a ferramenta ajudasse a organizar as informações produzidas durante o trabalho.

Um requisito importante era a **privacidade dos dados**: o código do usuário não poderia ser enviado a serviços externos, o que exigia que a inteligência artificial rodasse localmente.

---

<a id="solucao"></a>

<br>

## ✅ Solução

Desenvolvemos o **DeepCode**, uma aplicação desktop em **Java e JavaFX** em que o usuário digita um código e o envia para análise. O código é processado por um modelo de linguagem executado localmente pelo **Ollama** (Qwen 2.5 Coder), configurado para detectar, apontar e corrigir erros em exercícios de programação em Python.

A resposta da IA é exibida em uma tela própria e pode ser salva com um título em um banco **MySQL**. As respostas salvas ficam disponíveis em um menu lateral, onde podem ser filtradas, consultadas e excluídas.

### Principais funcionalidades

- Área para digitar o código, com botões de enviar e limpar.
- Envio do código ao modelo de IA executado localmente.
- Tela de resposta com data e hora, opção de gerar nova resposta, salvar e voltar.
- Salvamento das respostas com título no banco de dados.
- Menu lateral animado com as respostas salvas e filtro por nome.
- Consulta e exclusão do histórico, com confirmação.
- Barra de status com mensagens de retorno ao usuário.
- Tutorial em vídeo para instalação do ambiente.

### Organização da solução

| Componente | Responsabilidade |
|---|---|
| `gui/Main.java` | Interface JavaFX: telas, menu lateral e ações do usuário |
| `gui/application.css` | Tema visual da aplicação |
| `ia/IA.java` | Comunicação com o modelo de IA local pelo Ollama |
| `dao/HistoricoDAO.java` | Salvar, listar, consultar e excluir respostas no banco |
| `factory/ConnectionFactory.java` | Conexão com o banco MySQL |
| `Modelfile` | Configuração do modelo de IA e de suas instruções |

---

<a id="cronograma-e-entregas"></a>

<br>

## 📅 Cronograma e entregas

| Etapa | Período | Principais entregas | Situação |
|---|---|---|---|
| Kick-off | 24/02/2025 a 28/02/2025 | Apresentação do desafio e alinhamento inicial | Concluído |
| Sprint 1 | 10/03/2025 a 30/03/2025 | Wireframe no Figma, editor simples, integração com a IA, envio do código e resposta em área separada | Concluída |
| Sprint 2 | 07/04/2025 a 27/04/2025 | Atualização do protótipo e interface mais intuitiva, com navegação entre telas | Concluída |
| Sprint 3 | 05/05/2025 a 25/05/2025 | Armazenamento das respostas no banco, consulta do histórico e tutorial de instalação | Concluída |
| Feira de Soluções | 29/05/2025 | Apresentação do projeto e demonstração da solução desenvolvida | Concluída |

---

<a id="link-do-repositorio-git"></a>

<br>

## 🔗 Link do repositório Git

- [Repositório do DeepCode](https://github.com/API-DeepCode/API2)

---

<a id="preview-da-aplicacao"></a>

<br>

## 🖥️ Preview da aplicação

[▶️ Assistir ao tutorial de instalação](https://www.youtube.com/watch?v=vB7EBUyKuwA)

O vídeo mostra como preparar o ambiente para executar o DeepCode, com Java, JavaFX, MySQL e o modelo de IA local.

---

<a id="tecnologias-utilizadas"></a>

<br>

## 🛠️ Tecnologias utilizadas

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" width="48" height="48" alt="Java" title="Java">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" width="48" height="48" alt="CSS" title="CSS">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original.svg" width="48" height="48" alt="MySQL" title="MySQL">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/eclipse/eclipse-original.svg" width="48" height="48" alt="Eclipse" title="Eclipse">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/figma/figma-original.svg" width="48" height="48" alt="Figma" title="Figma">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/jira/jira-original.svg" width="48" height="48" alt="Jira" title="Jira">
</p>

| Área | Tecnologias | Aplicação no projeto |
|---|---|---|
| Linguagem | Java | Lógica da aplicação desktop |
| Interface | JavaFX e CSS | Telas, menu lateral, animações e tema visual |
| Inteligência artificial | Ollama e Qwen 2.5 Coder | Análise e correção do código, executadas localmente |
| Banco de dados | MySQL e JDBC | Armazenamento e consulta do histórico de respostas |
| Integração | HTTP e org.json | Comunicação com o modelo de IA |
| Prototipação | Figma | Wireframes e protótipo das telas |
| Gestão e colaboração | Jira, Eclipse, Git e GitHub | Backlog, burndown, desenvolvimento e versionamento |

---

<a id="contribuicoes-pessoais"></a>

<br>

## 👨‍💻 Contribuições pessoais

Atuei como **desenvolvedor**, com foco na **interface gráfica** da aplicação, do protótipo ao código.

Nas primeiras sprints, fiquei responsável pelo **wireframe no Figma**, por sua atualização e pela elaboração do design da tela principal. Em seguida, levei esse design para o código em **JavaFX**.

Na Sprint 2, separei a interface em **duas telas** — envio do código e resposta da IA —, com os botões de salvar e voltar, a validação de código vazio, o registro de data e hora da resposta e a janela para salvar a resposta com título. Também criei o **tema visual** da aplicação em CSS. Na sequência, reorganizei o layout para ser redimensionável e introduzi o **menu lateral** para acessar as respostas salvas.

Na Sprint 3, fiz o **redesenho completo da interface**: menu lateral animado com filtro por nome, cabeçalho, barra de status com mensagens de retorno, botão de limpar código, ícones nos botões e um novo tema com gradientes e efeitos ao passar o mouse.

A integração do menu lateral com o banco de dados, o botão de atualizar a lista e a janela de histórico com exclusão foram desenvolvidos por outros integrantes, a partir da estrutura de interface que eu havia criado. Em código, fui o principal autor da interface gráfica do projeto.

---

<a id="hard-skills"></a>

<br>

## 🧠 Hard skills

<details>
  <summary><strong>Clique para visualizar as hard skills desenvolvidas no projeto</strong></summary>

<br>

| Hard skill | Nível de proficiência | Evidência no projeto |
|---|---|---|
| Java | Sei fazer com autonomia | Lógica das telas e das ações da interface |
| JavaFX | Sei fazer com autonomia | Telas, layout redimensionável, menu lateral e animações |
| CSS para JavaFX | Sei fazer com autonomia | Tema visual com gradientes e efeitos de interação |
| Figma | Sei fazer com autonomia | Wireframe e protótipo das telas |
| UX e design de interfaces | Sei fazer com autonomia | Navegação em duas telas e mensagens de retorno ao usuário |
| MySQL e JDBC | Faço com ajuda | Integração da interface com o salvamento das respostas |
| Integração com IA local | Faço com ajuda | Exibição das respostas geradas pelo modelo no Ollama |
| Git e GitHub | Sei fazer com autonomia | Branch própria e pull requests para a principal |

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
| Criatividade | Propus o menu lateral e o novo visual da aplicação na última sprint |
| Atenção à experiência do usuário | Adicionei validação de código vazio e mensagens de status para orientar o usuário |
| Colaboração | Deixei a estrutura da interface pronta para que os colegas integrassem o banco de dados |
| Organização | Trabalhei em uma branch própria e integrei as entregas por pull requests |
| Iniciativa | Levei o protótipo do Figma para o código sem depender de outra pessoa |

</details>

---

<a id="aprendizados"></a>

<br>

## 📚 Aprendizados

O DeepCode foi meu primeiro projeto com uma aplicação desktop e com inteligência artificial. Trabalhar com um modelo de linguagem executado localmente mostrou como requisitos como a privacidade dos dados influenciam diretamente as decisões técnicas do projeto.

Ser responsável pela interface do protótipo ao código me ensinou a pensar no fluxo de uso antes da implementação. Separar o envio do código da resposta, dar retorno ao usuário pela barra de status e organizar o histórico no menu lateral foram decisões que tornaram a ferramenta mais simples de usar.

Também passei a trabalhar com branch própria e pull requests, o que reforçou a importância de integrar as entregas de forma organizada e de deixar o código preparado para que outros integrantes pudessem continuar a partir dele.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 1 • Os Python On](./API_1.md) | [➡️ API 3 • EntrenovaFlix](./API_3.md) |

</div>
