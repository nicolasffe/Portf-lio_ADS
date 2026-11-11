# API 4 - EchoCAD

<p align="center">
  <strong>4º Semestre • 2026-1</strong><br>
  Automatização de documentos técnicos de obras a partir de plantas CAD, com cálculos, preços SINAPI e IA<br>
  Papel exercido no Scrum: <strong>Desenvolvedor</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projeto%20Acad%C3%AAmico-Fatec%20SJC-blue?style=for-the-badge" alt="Projeto Acadêmico Fatec SJC">
  <img src="https://img.shields.io/badge/Tipo-Web%20com%20IA-informational?style=for-the-badge" alt="Aplicação web com IA">
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
| Semestre do curso | 4º semestre |
| Ano e semestre | 2026-1 |
| Nome do projeto | EchoCAD — Automatização de documentos técnicos |
| Tipo de sistema | Aplicação web com processamento de plantas CAD e inteligência artificial |
| Papel no Scrum | Desenvolvedor |
| Atuação técnica | Fullstack: frontend completo, autenticação, integração do processamento com a interface e geração de especificações com IA |
| Equipe | Equipe Echo |
| Metodologia | Scrum, com backlog priorizado, DoR, DoD, critérios de aceitação e pull requests por área |
| Situação do projeto | Concluído, com as três sprints entregues |

---

<a id="empresa-parceira"></a>

<br>

## 🏢 Empresa parceira

| Item | Descrição |
|---|---|
| Empresa parceira | Exército Brasileiro — Guarnição de Caçapava |
| Contexto do desafio | Elaboração de memoriais de cálculo e documentação técnica de obras de engenharia |
| Professor P2 | [Nome do professor] |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |

---

<a id="problema"></a>

<br>

## ❗ Problema

Produzir o memorial de cálculo e a documentação técnica de uma obra a partir de suas plantas CAD é um trabalho manual e demorado. É preciso levantar áreas, comprimentos e ambientes, calcular quantitativos, consultar preços de insumos e redigir especificações de acordo com as normas técnicas.

O desafio proposto foi extrair automaticamente os dados relevantes de uma planta CAD enviada pelo usuário e, com apoio de inteligência artificial, gerar um documento conforme as normas da ABNT e uma planilha de custos, tudo por meio de uma interface simples.

---

<a id="solucao"></a>

<br>

## ✅ Solução

Desenvolvemos o **EchoCAD**, uma aplicação web em que o usuário envia uma planta no formato **DXF** e recebe os documentos técnicos da obra.

O backend, em **FastAPI**, lê o arquivo com a biblioteca **ezdxf**, extrai entidades e camadas e calcula os quantitativos. Com esses dados, gera o **memorial de cálculo em Excel**, com os preços de insumos da tabela **SINAPI**. Em seguida, um modelo de linguagem — **Groq** na nuvem ou **Ollama** localmente — redige as **especificações técnicas** com referência às normas NBR, exportadas em **DOCX**.

Os projetos ficam salvos por usuário, com histórico, busca e acompanhamento do processamento em tempo real. A aplicação roda em contêineres Docker, com banco MariaDB.

### Principais funcionalidades

- Envio de planta CAD com validação do formato DXF.
- Extração de dados da planta e cálculos de engenharia.
- Geração do memorial de cálculo em XLSX, com abas por etapa da obra.
- Consulta de preços de insumos na tabela SINAPI.
- Geração de especificações técnicas com IA e exportação em DOCX.
- Acompanhamento do processamento em tempo real.
- Cadastro, login, alteração de senha e escolha do provedor de IA, com chave da API Groq própria de cada usuário armazenada de forma criptografada.
- Histórico de projetos com busca, visualização e exclusão.
- Consulta e cadastro de normas técnicas.
- Modo claro e escuro.

### Organização da solução

| Componente | Responsabilidade |
|---|---|
| Frontend (React + Vite) | Páginas de login, cadastro, envio, processamento, resultado, histórico e normas |
| Backend (FastAPI) | Autenticação, projetos, upload, processamento, memorial e especificações |
| Módulo Memorial | Cálculos a partir do DXF, preços SINAPI e preenchimento da planilha |
| Módulo Especificações Técnicas | Geração do texto com IA e montagem do documento DOCX |
| Banco de dados (MariaDB) | Usuários, projetos, plantas, relatórios e especificações |
| Docker Compose | Execução do banco, backend, frontend e, opcionalmente, Ollama e túnel Cloudflare |

---

<a id="cronograma-e-entregas"></a>

<br>

## 📅 Cronograma e entregas

| Etapa | Período | Principais entregas | Situação |
|---|---|---|---|
| Sprint 1 | 16/03/2026 a 05/04/2026 | Geração do memorial de cálculo básico e primeira versão da interface | Concluída |
| Sprint 2 | 13/04/2026 a 03/05/2026 | Assistente de IA, geração de especificações técnicas, salvamento de projetos e tela de normas | Parcialmente concluída |
| Sprint 3 | 11/05/2026 a 31/05/2026 | Autenticação, integração completa do processamento, exportação dos documentos e manuais | Concluída |
| Feira de Soluções | [DD/MM/2026] | Apresentação do projeto e demonstração da solução desenvolvida | Concluída |

---

<a id="link-do-repositorio-git"></a>

<br>

## 🔗 Link do repositório Git

- [Repositório do EchoCAD](https://github.com/EquipeEcho/EchoCAD)

---

<a id="preview-da-aplicacao"></a>

<br>

## 🖥️ Preview da aplicação

- [▶️ Assistir à demonstração da Sprint 1 (MVP)](https://youtu.be/TYSAJDFz9T0)
- [▶️ Assistir à demonstração da Sprint 3](https://www.youtube.com/watch?v=uGvk_viRp7I)

A primeira demonstração apresenta o MVP com a geração do memorial de cálculo. A da Sprint 3 mostra o fluxo completo: login, envio da planta, processamento, resultado com memorial e especificações técnicas e histórico de projetos.

---

<a id="tecnologias-utilizadas"></a>

<br>

## 🛠️ Tecnologias utilizadas

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg" width="48" height="48" alt="React" title="React">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" width="48" height="48" alt="TypeScript" title="TypeScript">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vitejs/vitejs-original.svg" width="48" height="48" alt="Vite" title="Vite">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" width="48" height="48" alt="Python" title="Python">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/fastapi/fastapi-original.svg" width="48" height="48" alt="FastAPI" title="FastAPI">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mariadb/mariadb-original.svg" width="48" height="48" alt="MariaDB" title="MariaDB">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/docker/docker-original.svg" width="48" height="48" alt="Docker" title="Docker">
</p>

| Área | Tecnologias | Aplicação no projeto |
|---|---|---|
| Frontend | React, TypeScript, Vite e React Router | Telas, navegação, rotas protegidas e tema claro/escuro |
| Backend | Python, FastAPI e Pydantic | Endpoints, validações e regras de negócio |
| Banco de dados | MariaDB, SQLAlchemy e Alembic | Persistência e controle das alterações do banco |
| Plantas CAD | ezdxf e NetworkX | Leitura do DXF e extração de entidades e ambientes |
| Planilhas e documentos | pandas, openpyxl e python-docx | Memorial de cálculo em XLSX e especificações em DOCX |
| Inteligência artificial | Groq (Llama 3.3 70B) e Ollama (Qwen 2.5) | Geração das especificações técnicas |
| Segurança | JWT, bcrypt e Fernet | Sessões, senhas e criptografia das chaves de API |
| Infraestrutura | Docker, Docker Compose e Cloudflare Tunnel | Execução dos serviços e acesso externo |
| Gestão e colaboração | Jira, Git e GitHub | Backlog, branches por área e pull requests |

---

<a id="contribuicoes-pessoais"></a>

<br>

## 👨‍💻 Contribuições pessoais

Atuei como **desenvolvedor fullstack**. Comecei pelo frontend e, ao longo das sprints, passei a trabalhar também no backend e na integração entre as camadas.

Na **Sprint 1**, criei a **primeira versão completa do frontend** em React, Vite e TypeScript, com as páginas de início, processamento, resultado e histórico, os componentes, o gerenciamento de estado e a estilização. Também implementei o **modo escuro** da aplicação.

Na **Sprint 2**, desenvolvi o **modal de salvamento de projeto** e a **tela de normas técnicas**, com o formulário de dados do projeto e do levantamento de campo.

Na **Sprint 3**, atuei de ponta a ponta:

- **Autenticação:** telas de login e cadastro, controle de sessão, rotas protegidas, encerramento de sessão expirada e ajustes nos endpoints de usuário.
- **Processamento:** criei a rota que integra o processamento do DXF à interface, com o progresso enviado em tempo real, e melhorei a ligação entre a leitura da planta e o preenchimento do memorial em Excel.
- **Especificações técnicas com IA:** integrei a geração das especificações ao fluxo de processamento e aprimorei o gerador com Groq, incluindo modelos alternativos e novas tentativas em caso de falha.
- **Conta do usuário:** alteração de senha e cadastro da chave Groq de cada usuário, armazenada criptografada.
- **Histórico:** busca, visualização e exclusão de projetos.
- **Interface:** redesenho das telas de processamento e resultado.

Também revisei e integrei pull requests da branch de frontend na principal. Na versão final, sou o segundo integrante com mais linhas de código no projeto.

---

<a id="hard-skills"></a>

<br>

## 🧠 Hard skills

<details>
  <summary><strong>Clique para visualizar as hard skills desenvolvidas no projeto</strong></summary>

<br>

| Hard skill | Nível de proficiência | Evidência no projeto |
|---|---|---|
| React, TypeScript e Vite | Sei fazer com autonomia | Criação do frontend completo da aplicação |
| CSS e design de interfaces | Sei fazer com autonomia | Estilização das páginas e modo escuro |
| Python e FastAPI | Sei fazer com autonomia | Rotas de processamento, usuários e especificações |
| Autenticação com JWT | Sei fazer com autonomia | Login, cadastro, sessão e rotas protegidas |
| Integração com LLMs | Sei fazer com autonomia | Geração das especificações com Groq, com alternativas e novas tentativas |
| Streaming de dados | Faço com ajuda | Progresso do processamento enviado em tempo real à interface |
| Criptografia de dados sensíveis | Faço com ajuda | Armazenamento criptografado da chave de API de cada usuário |
| SQLAlchemy e Alembic | Faço com ajuda | Migrations para os novos campos de usuário |
| Docker e Docker Compose | Faço com ajuda | Ambiente de desenvolvimento com os serviços da aplicação |
| Git e GitHub | Sei fazer com autonomia | Branches por área, pull requests e resolução de conflitos |

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
| Adaptabilidade | Passei do frontend para o backend quando a integração entre as camadas se tornou prioridade |
| Resolução de problemas | Recuperei o frontend e o tema escuro depois de um conflito de merge que os havia removido |
| Colaboração | Integrei o processamento desenvolvido por colegas à interface que construí |
| Responsabilidade | Corrigi problemas de sessão, histórico e exclusão de projetos antes da entrega final |
| Atenção à experiência do usuário | Mostrei o progresso do processamento em tempo real para o usuário não ficar sem retorno |

</details>

---

<a id="aprendizados"></a>

<br>

## 📚 Aprendizados

O EchoCAD foi o projeto em que mais avancei para o desenvolvimento fullstack. Ter construído o frontend me deu uma visão clara do que a interface precisava receber, e isso facilitou o trabalho de integrar o backend a ela na última sprint.

Trabalhar com um domínio técnico como engenharia civil mostrou a importância de entender o problema do cliente antes de codificar. Termos como memorial de cálculo, quantitativos e tabela SINAPI precisaram ser compreendidos para que a solução gerasse documentos úteis.

A integração com modelos de linguagem ensinou que a IA precisa de tratamento de falhas: limites de uso, respostas incompletas e indisponibilidade do serviço exigiram modelos alternativos e novas tentativas. Também aprendi a proteger dados sensíveis, como as chaves de API dos usuários.

Por fim, o fluxo com branches por área e pull requests reforçou a importância de integrar com frequência e de resolver conflitos com cuidado em uma equipe grande.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 3 • EntrenovaFlix](./API_3.md) | — |

</div>
