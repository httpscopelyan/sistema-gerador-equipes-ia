# Sistema Gerador de Equipes com IA

Sistema full stack em desenvolvimento para auxiliar gestores na criação, organização e análise de equipes para turnês, projetos nacionais e internacionais.

A plataforma integra inteligência artificial ao processo de formação de equipes, utilizando dados vindos de planilhas importadas pelo usuário. O principal objetivo é automatizar e facilitar uma tarefa que normalmente exige análise manual, cruzamento de informações e tomada de decisão cuidadosa.

> Este repositório é uma apresentação pública do projeto. O código-fonte original é privado por conter regras de negócio, dados sensíveis e informações internas.

---

## Visão Geral

O **Sistema Gerador de Equipes com IA** foi desenvolvido para apoiar gestores na organização de voluntários em equipes, considerando destinos, perfis comportamentais, regras internas e relacionamentos entre participantes.

A IA atua analisando os perfis dos usuários presentes na planilha, incluindo informações como o perfil DISC. Com base nesses dados e em regras específicas, como casais, vínculos e distribuição por destino, o sistema sugere equipes mais equilibradas para projetos nacionais e internacionais.

Mesmo com a automação, o gestor continua tendo controle total sobre as decisões, podendo revisar, editar, criar e reorganizar equipes manualmente.

---

## Principais Funcionalidades

* Importação de voluntários por planilhas;
* Análise de perfis com apoio de IA;
* Geração automática de equipes;
* Criação e edição manual de times;
* Organização por destinos nacionais e internacionais;
* Configuração de relacionamentos e regras específicas;
* Workspaces salvos automaticamente;
* Histórico de estados anteriores do sistema;
* Dashboards para análise de dados;
* Visualização de destinos e mapas;
* Exportação de equipes em `.txt`;
* Impressão em formato PDF;
* Tratamento e proteção de dados sensíveis.

---

## Tecnologias Utilizadas

### Backend

* Node.js
* TypeScript
* Express
* Sequelize
* PostgreSQL
* Processamento de planilhas
* Integração com n8n
* Integração com IA
* Geração de relatórios
* Gerenciamento de workspaces e cache de grupos

### Frontend

* React
* TypeScript
* Vite
* Zustand
* Styled Components
* Mapbox
* Dashboards interativos
* Interface SPA
* Gerenciamento de estado global

---

## Tela Inicial

A tela inicial apresenta uma visão geral do sistema e centraliza o acesso às principais áreas da plataforma.

O foco da interface é permitir que o gestor tenha uma navegação clara, visual e objetiva, mesmo lidando com uma lógica complexa por trás da geração de equipes.

<img width="1852" height="974" alt="Captura de tela 2026-06-17 110348" src="https://github.com/user-attachments/assets/2a3ab5e5-496f-4574-9624-d402650f8fe8" />

---

## Workspaces

O sistema conta com uma aba de **workspaces**, responsável por armazenar automaticamente os resultados anteriores.

Essa funcionalidade permite que o usuário retorne a estados antigos do sistema, funcionando quase como uma “máquina do tempo”. Isso facilita a comparação entre diferentes formações, a recuperação de decisões anteriores e a continuidade do trabalho sem perder progresso.

<img width="1854" height="971" alt="Captura de tela 2026-06-17 110414" src="https://github.com/user-attachments/assets/606a2faa-85aa-4748-a562-47b184b542b1" />

---

## Dashboards

O sistema também possui dashboards para facilitar a análise dos dados pelo gestor.

Essa área ajuda na visualização de informações importantes sobre voluntários, equipes, destinos e distribuição geral dos participantes. Mesmo com a IA sugerindo as formações, os dashboards tornam a conferência manual mais clara e estratégica.

<img width="1855" height="967" alt="Captura de tela 2026-06-17 110434" src="https://github.com/user-attachments/assets/9499b9a2-f127-433c-827c-50d2b718e824" />

---

## Importação de Voluntários

Na aba de voluntários, o usuário realiza o upload da planilha com os dados dos participantes.

Como o sistema trabalha com informações sensíveis, a segurança dos dados é uma parte importante do projeto. A aplicação foi pensada para tratar essas informações com cuidado durante o processo de importação, análise e geração das equipes.

<img width="1854" height="971" alt="Captura de tela 2026-06-17 110553" src="https://github.com/user-attachments/assets/49ada797-8539-4121-be5d-10d7bbea43b5" />

---

## Equipes Geradas

Após o processamento da planilha, os voluntários são listados em equipes formadas com apoio da IA.

Além da geração automática, o sistema também permite criar equipes manualmente, editar grupos existentes e ajustar a organização conforme a necessidade do projeto.

O gestor também pode exportar os dados em arquivo `.txt` ou imprimir as equipes em formato PDF, facilitando o uso das informações fora da plataforma.

---

## Como a IA Atua

A inteligência artificial funciona como uma ferramenta de apoio à decisão.

Ela analisa os dados dos voluntários e considera regras definidas para sugerir formações mais equilibradas. Entre os critérios considerados estão:

* Perfil comportamental DISC;
* Relacionamentos entre voluntários;
* Casais;
* Destinos nacionais e internacionais;
* Distribuição equilibrada de perfis;
* Regras internas de organização;
* Dados vindos diretamente da planilha importada.

A IA não substitui o gestor, mas reduz o trabalho repetitivo e oferece uma base mais inteligente para a tomada de decisão.

---

## Estrutura do Projeto

O Gestor de Equipes Nissi é composto por dois projetos principais:

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

## Status do Projeto

O sistema ainda está em produção/desenvolvimento.

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
