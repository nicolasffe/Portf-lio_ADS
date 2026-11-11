# API 3 - EntrenovaFlix

<p align="center">
  <strong>3º Semestre • 2025-2</strong><br>
  Diagnóstico inteligente de treinamentos e mercado, com relatório gerado por IA e plataforma de trilhas<br>
  Papel exercido no Scrum: <strong>Product Owner</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projeto%20Acad%C3%AAmico-Fatec%20SJC-blue?style=for-the-badge" alt="Projeto Acadêmico Fatec SJC">
  <img src="https://img.shields.io/badge/Tipo-Web%20com%20IA-informational?style=for-the-badge" alt="Aplicação web com IA">
  <img src="https://img.shields.io/badge/Papel-Product%20Owner-orange?style=for-the-badge" alt="Product Owner">
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
| Semestre do curso | 3º semestre |
| Ano e semestre | 2025-2 |
| Nome do projeto | EntrenovaFlix — Diagnóstico Inteligente de Treinamentos e Mercado |
| Tipo de sistema | Aplicação web com inteligência artificial |
| Papel no Scrum | Product Owner |
| Atuação técnica | Frontend: dashboard, design das telas, relatório da IA e fluxo de pagamento |
| Equipe | DeepCode |
| Metodologia | Scrum, com backlog priorizado, estimativas em pontos, DoR, DoD e Planning Poker |
| Situação do projeto | Concluído, com as três sprints entregues |

---

<a id="empresa-parceira"></a>

<br>

## 🏢 Empresa parceira

| Item | Descrição |
|---|---|
| Empresa parceira | [Entrenova](https://link-da-empresa) |
| Contexto do desafio | Diagnóstico organizacional e venda de trilhas de desenvolvimento para empresas |
| Professor P2 | [Nome do professor] |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |

---

<a id="problema"></a>

<br>

## ❗ Problema

A empresa parceira precisava entender os principais problemas de seus clientes antes de oferecer soluções de treinamento. Para isso, queria um formulário com perguntas definidas por ela, capaz de traçar um panorama geral da situação de cada organização.

A partir das respostas, o sistema deveria gerar automaticamente, com inteligência artificial, um relatório de diagnóstico personalizado. Esse relatório também deveria servir de porta de entrada comercial, levando o cliente a contratar trilhas de desenvolvimento.

---

<a id="solucao"></a>

<br>

## ✅ Solução

Desenvolvemos o **EntrenovaFlix**, uma aplicação web em **Next.js** na qual o gestor responde a um diagnóstico organizacional em quatro dimensões: **Pessoas e Cultura**, **Estrutura e Operações**, **Mercado e Clientes** e **Direção e Futuro**.

As respostas são armazenadas no **Firebase Firestore** e pontuadas para identificar pontos fortes e fracos. Em seguida, uma rota de API envia essa análise à **API da OpenAI**, que gera o relatório. O cliente vê uma dimensão gratuitamente e é convidado a desbloquear as demais ao contratar um dos planos (Ouro, Diamante ou Premium). O relatório também pode ser enviado por e-mail em PDF.

Depois da contratação, a empresa acessa uma plataforma de trilhas e aulas, com visões diferentes para administradores, gestores e funcionários.

### Principais funcionalidades

- Página inicial com apresentação do produto e depoimentos.
- Cadastro e login com Firebase Authentication e perfis Admin, Gestão e Funcionário.
- Formulário de diagnóstico unificado, com barra de progresso e perguntas de escolha única, múltipla, abertas e em escala.
- Pontuação das respostas e geração do relatório de diagnóstico com IA.
- Relatório com uma dimensão gratuita e as demais bloqueadas por uma chamada para contratação.
- Envio do relatório por e-mail em PDF.
- Página de planos com benefícios, funcionamento, preços e comparativo.
- Tela de pagamento simulada, com confirmação e desbloqueio do relatório completo.
- Chatbot de perguntas frequentes.
- Dashboard com trilhas e aulas, mandala de desenvolvimento, conquistas, gestão de colaboradores e configurações da empresa.

### Organização da solução

| Componente | Responsabilidade |
|---|---|
| `app/` | Páginas da aplicação (início, login, cadastro, formulário, relatório, planos, pagamento e dashboard) |
| `app/api/gerar-diagnostico` | Rota que recebe as respostas e solicita o relatório à IA |
| `app/lib/` | Integração com Firebase e pontuação do formulário |
| `components/` | Componentes do dashboard, do formulário, dos planos, do pagamento e da interface |
| `hooks/` | Serviço de IA e envio do relatório por e-mail |
| `Documentacao/` | Backlog e registro de cada sprint |

---

<a id="cronograma-e-entregas"></a>

<br>

## 📅 Cronograma e entregas

| Etapa | Período | Principais entregas | Situação |
|---|---|---|---|
| Sprint 1 | 08/09/2025 a 28/09/2025 | Formulário de diagnóstico inicial, relatório simples e formulário detalhado | Concluída |
| Sprint 2 | 06/10/2025 a 26/10/2025 | Formulário único em quatro dimensões, relatório com dimensão gratuita, e-mail automático, planos e chatbot | Concluída |
| Sprint 3 | 03/11/2025 a 23/11/2025 | Checkout, desbloqueio após pagamento, dashboard completo, aulas, conta do usuário e gestão de equipe | Concluída |
| Feira de Soluções | [DD/MM/2025] | Apresentação do projeto e demonstração da solução desenvolvida | Concluída |

---

<a id="link-do-repositorio-git"></a>

<br>

## 🔗 Link do repositório Git

- [Repositório do EntrenovaFlix](https://github.com/API-DeepCode/API3_Entrenova)

---

<a id="preview-da-aplicacao"></a>

<br>

## 🖥️ Preview da aplicação

[▶️ Assistir à demonstração](https://link-do-video)

[Breve descrição do que o vídeo mostra.]

---

<a id="tecnologias-utilizadas"></a>

<br>

## 🛠️ Tecnologias utilizadas

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" width="48" height="48" alt="TypeScript" title="TypeScript">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg" width="48" height="48" alt="React" title="React">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nextjs/nextjs-original.svg" width="48" height="48" alt="Next.js" title="Next.js">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg" width="48" height="48" alt="Tailwind CSS" title="Tailwind CSS">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/firebase/firebase-original.svg" width="48" height="48" alt="Firebase" title="Firebase">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/storybook/storybook-original.svg" width="48" height="48" alt="Storybook" title="Storybook">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/figma/figma-original.svg" width="48" height="48" alt="Figma" title="Figma">
</p>

| Área | Tecnologias | Aplicação no projeto |
|---|---|---|
| Frontend | Next.js, React e TypeScript | Páginas, rotas e componentes da aplicação |
| Interface | Tailwind CSS, shadcn/ui, Radix UI, lucide-react e Recharts | Componentes visuais, ícones e gráficos do dashboard |
| Formulários | React Hook Form e Zod | Captura e validação das respostas |
| Dados e autenticação | Firebase Firestore e Firebase Authentication | Armazenamento das respostas, cadastro e login |
| Inteligência artificial | API da OpenAI | Geração do relatório de diagnóstico |
| E-mail e documentos | Nodemailer e PDFKit | Envio do relatório em PDF por e-mail |
| Documentação de componentes | Storybook | Catálogo e teste visual de componentes |
| Gestão e colaboração | Jira, Notion, Figma, Git e GitHub | Backlog, prototipação, pull requests e versionamento |

---

<a id="contribuicoes-pessoais"></a>

<br>

## 👨‍💻 Contribuições pessoais

Atuei como **Product Owner** da equipe DeepCode. Fui responsável pelo backlog do produto, com as user stories priorizadas e estimadas em pontos, e pelo alinhamento das entregas com o que a empresa parceira esperava em cada sprint. Também revisei e integrei pull requests da equipe na branch principal.

Além do papel de PO, contribuí diretamente com o código, principalmente no **frontend** da Sprint 3:

- **Dashboard:** criei a área logada da plataforma, com o menu filtrado pelo perfil do usuário e as páginas de trilhas e aulas, player de aula, mandala de desenvolvimento, conquistas, gestores, gestão de colaboradores, configurações da empresa e do funcionário, comentários e visões comercial, de atendimento e estratégica.
- **Página inicial do dashboard:** desenvolvi a apresentação, a linha do tempo de planejamento em cinco etapas e o painel de boas-vindas.
- **Design:** padronizei as cores da aplicação e redesenhei a página inicial, o login, o cadastro, o formulário e a página de planos.
- **Relatório da IA:** redesenhei a tela de resposta, com a dimensão gratuita e o bloqueio das demais, e criei a página de confirmação de pagamento que libera o relatório completo.
- **Pagamento:** reformulei o design da tela de pagamento criada por outro integrante e a integrei aos planos.
- **Componentes:** configurei o Storybook e criei o novo chatbot e o carrossel de depoimentos.

A lógica de pontuação e o prompt da inteligência artificial foram desenvolvidos por outros integrantes; minha parte se concentrou na experiência do usuário e na integração das telas com esse fluxo.

---

<a id="hard-skills"></a>

<br>

## 🧠 Hard skills

<details>
  <summary><strong>Clique para visualizar as hard skills desenvolvidas no projeto</strong></summary>

<br>

| Hard skill | Nível de proficiência | Evidência no projeto |
|---|---|---|
| React e Next.js | Sei fazer com autonomia | Criação do dashboard e das páginas da aplicação |
| TypeScript | Sei fazer com autonomia | Tipagem dos componentes e das telas |
| Tailwind CSS e shadcn/ui | Sei fazer com autonomia | Padronização visual e componentes da interface |
| Firebase | Faço com ajuda | Integração das telas com autenticação e dados |
| Storybook | Faço com ajuda | Configuração e criação de stories de componentes |
| Integração com IA | Faço com ajuda | Exibição do relatório gerado pela OpenAI |
| Gestão de backlog | Sei fazer com autonomia | Priorização e estimativa das user stories como PO |
| Git, GitHub e pull requests | Sei fazer com autonomia | Revisão e integração das branches da equipe |

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
| Liderança | Conduzi a priorização do backlog e o acompanhamento das entregas como Product Owner |
| Comunicação | Traduzi as necessidades da empresa parceira em user stories para a equipe |
| Tomada de decisão | Defini o que entraria em cada sprint considerando valor de negócio e esforço |
| Colaboração | Integrei pull requests de diferentes integrantes e evoluí telas iniciadas por colegas |
| Visão de produto | Pensei o relatório gratuito como etapa comercial que leva à contratação dos planos |

</details>

---

<a id="aprendizados"></a>

<br>

## 📚 Aprendizados

Ser Product Owner me mostrou que o produto precisa fazer sentido para o negócio, não apenas funcionar. O relatório gerado por IA não era só uma funcionalidade técnica: era a porta de entrada para a venda das trilhas, e isso orientou decisões como liberar apenas uma dimensão gratuitamente.

Conciliar o papel de PO com o desenvolvimento foi um desafio de organização. Aprendi a separar os momentos de decidir prioridades dos momentos de implementar, e a usar o backlog, o DoR e o DoD como referência para não perder o foco do que tinha sido combinado.

Tecnicamente, foi meu primeiro projeto grande com Next.js, TypeScript e uma biblioteca de componentes. Construir o dashboard reforçou a importância de componentes reutilizáveis e de um padrão visual único em uma aplicação com muitas telas.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 2 • DeepCode](./API_2.md) | [➡️ API 4 • EchoCAD](./API_4.md) |

</div>
