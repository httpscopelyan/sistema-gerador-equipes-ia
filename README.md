# Sistema Gerador de Equipes com IA

Sistema full stack em desenvolvimento para auxiliar gestores na criação, organização e análise de equipes para turnês, projetos nacionais e internacionais.

A plataforma integra inteligência artificial ao processo de formação de equipes, utilizando dados vindos de planilhas importadas pelo usuário. O principal objetivo é automatizar e facilitar uma tarefa que normalmente exige análise manual, cruzamento de informações, leitura de perfis e tomada de decisão cuidadosa por parte da gestão.

> Este repositório é uma apresentação pública do projeto. O código-fonte original é privado por conter regras de negócio, dados sensíveis e informações internas.

---

## Visão Geral

O sistema trabalha a partir de planilhas baixadas e enviadas pelo usuário. Esses dados são processados e utilizados para gerar equipes com apoio de IA, considerando perfis comportamentais, regras de relacionamento, casais, destinos nacionais e internacionais e critérios internos definidos para o projeto.

A IA atua como uma ferramenta de apoio à decisão, analisando os perfis dos voluntários por meio de dados como o perfil DISC e sugerindo formações mais equilibradas. Mesmo com a automação, o gestor mantém controle total para revisar, editar, criar ou reorganizar as equipes manualmente.

---

## Funcionalidades Principais

* Importação de voluntários por planilhas;
* Análise de perfis com apoio de IA;
* Geração automática de equipes;
* Criação e edição manual de times;
* Organização por destinos nacionais e internacionais;
* Configuração de relacionamentos e regras específicas;
* Controle de casais e vínculos entre voluntários;
* Workspaces salvos automaticamente;
* Histórico de estados anteriores do sistema;
* Dashboards para análise de dados;
* Visualização de destinos e mapas;
* Exportação de equipes em `.txt`;
* Impressão em formato PDF;
* Tratamento e proteção de dados sensíveis.

---

## Screenshots do Projeto

<img width="1852" height="974" alt="Captura de tela 2026-06-17 110348" src="https://github.com/user-attachments/assets/2a3ab5e5-496f-4574-9624-d402650f8fe8" />

### Workspaces

O sistema ainda em produção contém uma aba de **workspaces**, responsável por guardar automaticamente os resultados anteriores.

Essa funcionalidade permite que o usuário retorne a estados antigos do sistema, funcionando quase como uma “máquina do tempo”. Isso facilita a comparação entre diferentes formações, a recuperação de decisões anteriores e a continuidade do trabalho sem perder progresso.

---

<img width="1854" height="971" alt="Captura de tela 2026-06-17 110414" src="https://github.com/user-attachments/assets/606a2faa-85aa-4748-a562-47b184b542b1" />

### Dashboards

O sistema contém dashboards que ajudam o gestor a analisar os dados e verificar manualmente suas escolhas e decisões.

Essa área facilita a visualização de informações importantes sobre voluntários, equipes, destinos e distribuição geral dos participantes. Mesmo com a IA sugerindo formações, os dashboards tornam a conferência mais clara, visual e estratégica.

---

<img width="1855" height="967" alt="Captura de tela 2026-06-17 110434" src="https://github.com/user-attachments/assets/9499b9a2-f127-433c-827c-50d2b718e824" />

### Importação de Voluntários

Na aba de voluntários, o usuário realiza o upload da planilha contendo os dados dos participantes.

Como o sistema trabalha com dados sensíveis, a segurança é uma parte importante do projeto. A aplicação foi pensada para tratar essas informações com cuidado durante o processo de importação, análise, geração de equipes e armazenamento dos dados.

---

<img width="1854" height="971" alt="Captura de tela 2026-06-17 110553" src="https://github.com/user-attachments/assets/49ada797-8539-4121-be5d-10d7bbea43b5" />

### Equipes Geradas

Nesta área, os usuários importados da planilha são listados em equipes formadas com apoio da IA.

Além da geração automática, o sistema também permite criar equipes manualmente, editar grupos já existentes e ajustar a organização conforme a necessidade do projeto. Também é possível baixar as equipes em arquivo `.txt` ou imprimir em formato PDF.

---

## Estrutura do Projeto

O **Gestor de Equipes Nissi** é composto por dois projetos principais:

### Backend — `nissi-api`

API desenvolvida com Node.js, TypeScript, Express, Sequelize e PostgreSQL.

Responsável por:

* Processar planilhas de voluntários;
* Validar e organizar dados;
* Enviar dados para o n8n;
* Integrar com IA;
* Gerar equipes;
* Salvar workspaces;
* Gerenciar cache de grupos;
* Criar relatórios;
* Persistir informações no banco de dados.

### Frontend — `gestor_de_equipesNissi`

SPA desenvolvida com React, TypeScript, Vite, Zustand e Styled Components.

Responsável por:

* Abrir e gerenciar workspaces;
* Importar voluntários;
* Gerar equipes;
* Visualizar dashboards;
* Editar equipes;
* Configurar relacionamentos;
* Exibir destinos e mapas;
* Gerenciar relatórios;
* Exportar e imprimir informações.

---

## Tecnologias Utilizadas

### Frontend

* React
* TypeScript
* Vite
* Zustand
* Styled Components
* Mapbox

### Backend

* Node.js
* TypeScript
* Express
* Sequelize
* PostgreSQL
* n8n
* Integração com IA

---

## Status do Projeto

O sistema ainda está em desenvolvimento.

Algumas funcionalidades já estão implementadas e em fase de ajuste, enquanto outras áreas continuam sendo desenvolvidas e aprimoradas.

### Em andamento

* Melhorias na geração automática de equipes;
* Refinamento das regras de IA;
* Expansão dos relatórios;
* Melhorias nos dashboards;
* Ajustes na experiência do usuário;
* Otimização da segurança e tratamento de dados;
* Novas ferramentas de edição manual.

---

## Objetivo

O objetivo principal do projeto é transformar um processo manual, demorado e sujeito a erros em uma experiência mais rápida, visual e inteligente.

Com apoio da IA, o gestor consegue analisar melhor os perfis dos voluntários, organizar equipes com mais clareza e tomar decisões mais estratégicas para diferentes tipos de turnês, projetos e destinos.

---

## Observação

O restante do sistema continua em desenvolvimento.

Por conter dados sensíveis, regras de negócio e informações internas, este repositório funciona apenas como apresentação pública do projeto para fins de portfólio.
