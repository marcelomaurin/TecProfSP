# TecProfSP

![Status](https://img.shields.io/badge/status-em%20planejamento-blue)
![Plataforma](https://img.shields.io/badge/plataforma-Raspberry%20Pi-red)
![Ambiente](https://img.shields.io/badge/ambiente-Linux%20modo%20texto-black)
![Web](https://img.shields.io/badge/web-Apache%20%2B%20PHP-orange)
![Linguagens](https://img.shields.io/badge/linguagens-Python%20%7C%20Bash%20%7C%20C%2FGCC-green)
![Banco de Dados](https://img.shields.io/badge/bancos-MySQL%20%7C%20PostgreSQL-blueviolet)
![Acesso](https://img.shields.io/badge/acesso-SSH%20%7C%20Browser-success)

> Ferramenta de desenvolvimento didático para apoiar professores técnicos no ensino de disciplinas de informática.

---

## Sumário

- [1. Apresentação](#1-apresentação)
- [2. Conceito do projeto](#2-conceito-do-projeto)
- [3. Objetivo geral](#3-objetivo-geral)
- [4. Público-alvo](#4-público-alvo)
- [5. Disciplinas apoiadas](#5-disciplinas-apoiadas)
- [6. Funcionamento do ambiente](#6-funcionamento-do-ambiente)
- [7. Perfis de acesso](#7-perfis-de-acesso)
- [8. Tecnologias previstas](#8-tecnologias-previstas)
- [9. Estrutura pedagógica](#9-estrutura-pedagógica)
- [10. Implantação do servidor](#10-implantação-do-servidor)
- [11. Renovação anual](#11-renovação-anual)
- [12. Capacidade planejada](#12-capacidade-planejada)
- [13. Benefícios esperados](#13-benefícios-esperados)
- [14. Estrutura sugerida do repositório](#14-estrutura-sugerida-do-repositório)
- [15. Possibilidades futuras](#15-possibilidades-futuras)
- [16. Autor](#16-autor)

---

## 1. Apresentação

O **TecProfSP** é um projeto educacional idealizado por **Marcelo Maurin Martins**, **Professor Técnico do Estado de São Paulo**, com a proposta de disponibilizar um **servidor local de desenvolvimento didático** para uso em aulas técnicas de informática.

O projeto foi concebido para auxiliar professores técnicos no processo de ensino prático, oferecendo aos alunos um ambiente controlado, acessível e voltado ao desenvolvimento de competências reais em tecnologia.

---

## 2. Conceito do projeto

O **TecProfSP não é apenas uma imagem isolada**, mas sim uma **ferramenta de desenvolvimento usada pelos professores técnicos para lecionar disciplinas técnicas de informática**.

A base do projeto é um **servidor local**, executado em equipamento compatível com **Raspberry Pi**, que disponibiliza um ambiente Linux em **modo texto**, sem interface gráfica, acessível por navegador e também por SSH.

Esse servidor funciona como um laboratório prático local, permitindo que os alunos treinem, desenvolvam atividades e utilizem ferramentas reais de informática em um ambiente pedagógico preparado pelo professor.

---

## 3. Objetivo geral

Criar um **servidor local educacional** para apoiar o desenvolvimento das aptidões técnicas dos alunos, permitindo o uso prático de ferramentas de desenvolvimento, bancos de dados, programação e administração de ambientes Linux.

O foco do projeto é dar suporte ao professor técnico, oferecendo uma infraestrutura simples e funcional para aulas práticas de informática.

---

## 4. Público-alvo

O projeto é voltado para:

- alunos de cursos técnicos profissionalizantes;
- professores técnicos da área de informática;
- escolas e laboratórios de ensino técnico;
- turmas com necessidade de ambiente local de treinamento prático.

---

## 5. Disciplinas apoiadas

O servidor TecProfSP foi pensado para apoiar principalmente disciplinas como:

- **Processamento de Dados**;
- **Modelagem de Dados**;
- **Programação em Python**;
- **Ferramentas Linux**;
- **Scripts Bash**;
- práticas introdutórias com compilação em **C usando GCC**;
- uso de bancos de dados relacionais em ambiente didático.

---

## 6. Funcionamento do ambiente

O TecProfSP funcionará como um **servidor local de uso didático**, com recursos acessíveis por meio de interface web e terminal.

### Recursos principais do ambiente

- interface web em **PHP** executada em **Apache**;
- acesso a tarefas disponibilizadas pelo professor;
- terminal no navegador utilizando a **conta SSH do próprio aluno**;
- uso de ferramentas para treinamento técnico;
- acesso controlado a pequenos ambientes de banco de dados individuais;
- execução de programas em **Python**;
- uso de **Bash** e comandos Linux;
- uso de compilação em **C com GCC**;
- acesso ao **Moodle**, com aulas práticas preparadas pelo professor.

### Fluxo de uso do aluno

1. O aluno acessa a interface do sistema.
2. Visualiza a tarefa proposta pelo professor.
3. Utiliza uma tela no navegador para desenvolver a atividade.
4. Essa tela opera com a **conta SSH do próprio aluno**.
5. O aluno utiliza as ferramentas disponibilizadas para treinamento.
6. Quando necessário, acessa o **Moodle** para consultar aulas práticas, roteiros e materiais preparados pelo professor.

---

## 7. Perfis de acesso

O sistema deverá possuir perfis distintos, com separação de permissões.

### Aluno

- acesso ao ambiente web;
- acesso ao terminal associado à sua própria conta;
- uso de ferramentas liberadas para aula;
- armazenamento dos seus arquivos e exercícios;
- acesso aos seus bancos de dados individuais;
- acesso ao Moodle.

### Professor

- gerenciamento de atividades e tarefas;
- organização das turmas;
- acompanhamento do uso do ambiente;
- preparação de conteúdos práticos;
- acesso ampliado ao ambiente didático;
- integração com o Moodle.

### Administrador

- manutenção completa do servidor;
- criação e remoção de contas;
- configuração de Apache, PHP, SSH e bancos de dados;
- atualização técnica do ambiente;
- geração da nova mídia anual do sistema.

---

## 8. Tecnologias previstas

O projeto deverá utilizar tecnologias como:

- **Linux**;
- **Apache**;
- **PHP**;
- **Python**;
- **Bash**;
- **GCC**;
- **MySQL**;
- **PostgreSQL**;
- **SSH**;
- **Moodle**;
- bibliotecas de desenvolvimento e apoio didático.

---

## 9. Estrutura pedagógica

O TecProfSP busca oferecer uma experiência prática de ensino, permitindo que o professor conduza atividades reais em um ambiente técnico controlado.

O aluno poderá:

- praticar comandos Linux;
- desenvolver scripts em Bash;
- programar em Python;
- compilar programas simples em C;
- criar estruturas de banco de dados;
- testar consultas em MySQL e PostgreSQL;
- desenvolver exercícios práticos diretamente no navegador;
- acompanhar materiais complementares no Moodle.

---

## 10. Implantação do servidor

Para utilização do **TecProfSP**, será necessário:

- baixar a imagem oficial do projeto;
- utilizar o **Win32 Disk Imager** para gravar a imagem;
- preparar um cartão de **32 GB ou maior**;
- inserir o cartão no Raspberry Pi para inicialização do servidor local.

A gravação da imagem deverá ser feita de forma padronizada, para garantir que os ambientes educacionais mantenham a mesma base técnica e pedagógica.

### Armazenamento mínimo

- cartão de **32 GB ou maior**.

Esse armazenamento será utilizado para conter:

- sistema operacional;
- ambiente web;
- ferramentas de desenvolvimento;
- bancos de dados;
- bibliotecas;
- estrutura de usuários;
- tarefas e materiais didáticos.

---

## 11. Renovação anual

Ao final de cada ano letivo, deverá ser gerada uma **nova mídia do sistema**, permitindo:

- renovação completa do ambiente;
- limpeza de dados antigos;
- atualização de bibliotecas e ferramentas;
- reorganização das turmas;
- preparação do servidor para o novo ciclo letivo.

---

## 12. Capacidade planejada

Cada servidor deverá permitir o atendimento de até:

- **45 alunos por servidor**.

Essa capacidade foi pensada para atender turmas de ensino técnico com uso compartilhado e organizado dos recursos.

---

## 13. Benefícios esperados

- apoio prático ao ensino técnico;
- fortalecimento das aulas de informática aplicada;
- padronização do ambiente de desenvolvimento;
- maior contato dos alunos com ferramentas reais;
- formação orientada à prática profissional;
- baixo custo de implantação;
- facilidade de replicação em diferentes unidades;
- suporte ao professor técnico em atividades práticas.

---

## 14. Estrutura sugerida do repositório

```text
TecProfSP/
├── README.md
├── docs/
│   ├── apresentacao.md
│   ├── objetivos.md
│   ├── arquitetura.md
│   └── planejamento.md
├── imagem/
│   ├── configuracao_sistema.md
│   ├── pacotes_instalados.md
│   └── renovacao_anual.md
├── web/
│   ├── cadastro_alunos/
│   ├── acesso_alunos/
│   ├── acesso_professor/
│   └── ferramentas/
├── banco/
│   ├── mysql/
│   ├── postgres/
│   └── modelos/
├── moodle/
│   └── integracao/
├── scripts/
│   ├── criacao_usuarios/
│   ├── backup/
│   └── manutencao/
└── aulas/
    ├── processamento_de_dados/
    ├── modelagem_de_dados/
    ├── python/
    └── linux/
```

---

## 15. Possibilidades futuras

Entre as expansões futuras do projeto, podem ser consideradas:

- painel administrativo mais avançado para professores;
- relatórios de uso por turma;
- automação de criação de contas;
- integração ampliada com o Moodle;
- inclusão de novos compiladores e linguagens;
- monitoramento de uso do ambiente;
- criação de roteiros automáticos por atividade.

---

## 16. Autor

**Marcelo Maurin Martins**  
Professor Técnico do Estado de São Paulo

---

## Resumo

O **TecProfSP** é um projeto educacional voltado à criação de um **servidor local de desenvolvimento didático**, executado em equipamento compatível com **Raspberry Pi**, para apoiar professores técnicos no ensino de disciplinas de informática. O ambiente funciona em **modo texto**, sem interface gráfica, utilizando **Apache**, **PHP**, **Python**, **Bash**, **GCC**, **MySQL**, **PostgreSQL**, **SSH** e **Moodle**. Os alunos acessam tarefas por uma interface web, utilizam um terminal no navegador com sua própria conta SSH e treinam em um ambiente real de desenvolvimento preparado pelo professor.
