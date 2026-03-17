# Planejamento do Projeto TecProfSP

## 1. Visão geral

O **TecProfSP** é uma ferramenta acadêmica voltada ao apoio do ensino técnico em informática, estruturada sobre um servidor local de baixo custo, com ambiente controlado, seguro e previamente configurado para uso em escola.

A proposta do planejamento é organizar, em alto nível, as etapas necessárias para construção, validação e implantação da ferramenta, permitindo evolução gradual e sustentável do projeto.

---

## 2. Objetivo do planejamento

Este documento apresenta as etapas de construção da ferramenta e um plano de execução orientado por entregas progressivas.

A ideia central é desenvolver o projeto em blocos funcionais, iniciando pela base técnica do servidor e avançando até os recursos pedagógicos, administrativos e operacionais.

---

## 3. Princípios de execução

Para que o projeto seja viável em ambiente escolar, o desenvolvimento deve seguir alguns princípios:

- **baixo custo de implantação**;
- **simplicidade de manutenção**;
- **uso de tecnologias estáveis e amplamente conhecidas**;
- **estrutura modular**;
- **foco em ambiente textual e web leve**;
- **segurança no acesso dos usuários**;
- **facilidade de replicação em outras unidades escolares**;
- **prioridade para uso prático em sala de aula**.

---

## 4. Etapas da construção da ferramenta

## Etapa 1 — Definição do escopo pedagógico e técnico

Nesta etapa, o foco é consolidar o propósito da ferramenta, os perfis de usuários e os recursos mínimos necessários.

### Entregas esperadas
- definição do objetivo acadêmico da ferramenta;
- definição dos perfis de acesso: aluno, professor e administrador;
- definição das disciplinas inicialmente atendidas;
- definição da capacidade por servidor;
- definição do modelo de uso em ambiente escolar.

### Resultado esperado
Uma visão clara do que será implantado, para quem e com qual finalidade didática.

---

## Etapa 2 — Estruturação da base do servidor

Nesta fase, será preparada a base do servidor local que sustentará toda a solução.

### Atividades principais
- preparação do sistema Linux em modo texto;
- configuração do acesso remoto e administração básica;
- definição da política de usuários e permissões;
- organização do armazenamento local;
- estruturação do modelo de instalação e replicação do ambiente.

### Resultado esperado
Servidor funcional, estável e padronizado, pronto para receber os serviços do projeto.

---

## Etapa 3 — Implantação dos serviços principais

Com o servidor pronto, devem ser instalados e configurados os serviços centrais da plataforma.

### Atividades principais
- configuração do servidor web;
- configuração da aplicação em PHP;
- configuração de acesso via SSH;
- instalação e preparação dos bancos de dados MySQL e PostgreSQL;
- instalação das ferramentas de programação e compilação;
- disponibilização de ambiente para Python, Bash e GCC.

### Resultado esperado
Ambiente técnico preparado para uso didático, com os principais recursos operacionais disponíveis.

---

## Etapa 4 — Construção da interface acadêmica

Nesta etapa será desenvolvida a camada de interação com os usuários.

### Atividades principais
- criação da interface web de autenticação;
- criação da interface de cadastro e gestão de alunos;
- criação da interface de acesso do professor;
- criação da interface do aluno com visualização de tarefas;
- integração de terminal no navegador vinculado à conta individual do aluno;
- disponibilização dos atalhos para ferramentas de apoio acadêmico.

### Resultado esperado
Ambiente de uso simples, acessível e organizado, permitindo que aluno e professor interajam com a ferramenta de forma prática.

---

## Etapa 5 — Preparação do ambiente individual do aluno

Cada aluno deverá ter um espaço isolado e seguro para desenvolvimento das atividades propostas.

### Atividades principais
- criação automatizada de contas;
- estruturação de diretórios individuais;
- definição de permissões restritas por perfil;
- disponibilização de pequenos bancos de dados individuais;
- configuração do ambiente de terminal e desenvolvimento do aluno.

### Resultado esperado
Cada estudante com ambiente próprio, controlado e preparado para treinamento técnico sem interferência entre usuários.

---

## Etapa 6 — Integração pedagógica

Com a base técnica pronta, a ferramenta deve se aproximar da prática de sala de aula.

### Atividades principais
- integração com o Moodle;
- disponibilização de aulas práticas preparadas pelo professor;
- organização das tarefas por disciplina;
- definição de roteiros práticos de uso;
- montagem de exemplos de exercícios em Linux, banco de dados e programação.

### Resultado esperado
Ferramenta alinhada ao conteúdo acadêmico, apoiando efetivamente o processo de ensino-aprendizagem.

---

## Etapa 7 — Testes e validação em ambiente escolar

Antes da implantação definitiva, a solução deve ser validada em cenário real de uso.

### Atividades principais
- testes de autenticação e permissões;
- testes de acesso concorrente por múltiplos alunos;
- testes das interfaces web;
- testes dos ambientes individuais;
- testes das ferramentas de banco de dados, programação e terminal;
- validação da navegação do aluno e do professor.

### Resultado esperado
Maior confiabilidade da solução e identificação prévia de ajustes necessários.

---

## Etapa 8 — Implantação piloto

Após a validação, o projeto deve ser implantado inicialmente em escala controlada.

### Atividades principais
- preparação de um servidor piloto;
- cadastro inicial de turmas;
- treinamento básico de uso pelo professor;
- aplicação em atividades acadêmicas reais;
- coleta de observações e pontos de melhoria.

### Resultado esperado
Primeira versão funcional em uso acadêmico, com base concreta para expansão futura.

---

## Etapa 9 — Padronização e replicação

Após o piloto, a ferramenta deve ser organizada para uso contínuo e replicável.

### Atividades principais
- documentação técnica e operacional;
- documentação pedagógica;
- padronização do processo de instalação;
- definição da rotina de geração de nova mídia anual;
- organização de backups e manutenção;
- preparação para replicação em outras turmas ou unidades.

### Resultado esperado
Projeto maduro, documentado e apto a continuidade institucional.

---

## 5. Plano de execução proposto

A execução pode ser organizada em fases progressivas.

## Fase 1 — Fundação do ambiente
**Foco:** base do servidor e serviços principais.

### Meta
Entregar um servidor local funcional, com Linux em modo texto, SSH, Apache, PHP, MySQL, PostgreSQL, Python, Bash e GCC.

### Prioridades
- sistema base;
- usuários e permissões;
- serviços de infraestrutura;
- validação de estabilidade.

---

## Fase 2 — Camada acadêmica inicial
**Foco:** disponibilizar acesso ao aluno e ao professor.

### Meta
Entregar interface web com autenticação, cadastro de alunos e acesso ao ambiente individual.

### Prioridades
- interface administrativa;
- interface do aluno;
- terminal no navegador;
- organização das contas por perfil.

---

## Fase 3 — Ferramentas didáticas e integração
**Foco:** aproximar o ambiente do uso pedagógico real.

### Meta
Disponibilizar tarefas, ferramentas acadêmicas e integração com o Moodle.

### Prioridades
- tarefas por aluno;
- acesso às aulas práticas;
- bancos individuais;
- materiais de apoio;
- rotinas de uso pelo professor.

---

## Fase 4 — Consolidação e piloto
**Foco:** testar a solução com turma real.

### Meta
Executar implantação controlada em ambiente escolar e medir o comportamento da plataforma.

### Prioridades
- testes de carga;
- testes de usabilidade;
- coleta de melhorias;
- ajustes operacionais.

---

## Fase 5 — Expansão e manutenção anual
**Foco:** garantir continuidade e reaproveitamento institucional.

### Meta
Padronizar geração de nova mídia anual, manutenção e reaplicação da ferramenta em novos ciclos letivos.

### Prioridades
- documentação;
- geração da nova imagem anual;
- atualização das ferramentas;
- limpeza e reorganização do ambiente;
- replicação do projeto.

---

## 6. Cronograma de alto nível

## Curto prazo
- consolidar documentação do projeto;
- definir arquitetura final;
- preparar o servidor base;
- instalar os serviços principais;
- validar ambiente em modo texto.

## Médio prazo
- desenvolver a interface web;
- estruturar o cadastro de alunos;
- preparar o terminal no navegador;
- configurar ambientes individuais;
- integrar bancos de dados e ferramentas didáticas.

## Médio prazo avançado
- integrar Moodle;
- cadastrar tarefas acadêmicas;
- montar atividades práticas;
- testar o uso com alunos;
- realizar ajustes de segurança e usabilidade.

## Longo prazo
- implantar piloto com turma real;
- consolidar documentação técnica e pedagógica;
- definir rotina anual de renovação do ambiente;
- preparar o projeto para replicação em outras turmas e escolas.

---

## 7. Vantagens do modelo de execução

A construção por etapas oferece vantagens importantes:

- reduz complexidade inicial;
- permite validar cada bloco antes de avançar;
- facilita manutenção e correções;
- favorece reaproveitamento de conhecimento já consolidado;
- torna o projeto mais compatível com a realidade de escola pública;
- permite crescimento gradual conforme disponibilidade de tempo e recursos.

---

## 8. Resultado esperado

Ao final da execução, espera-se obter uma ferramenta acadêmica prática, padronizada e de baixo custo, capaz de oferecer aos alunos um ambiente real de treinamento técnico.

O resultado desejado é um servidor local educacional que permita:

- acesso controlado por perfis;
- uso de terminal e ferramentas reais de desenvolvimento;
- apoio ao ensino de Linux, banco de dados e programação;
- integração com materiais preparados pelo professor;
- aplicação prática em contexto escolar.

---

## 9. Considerações finais

O planejamento do TecProfSP deve priorizar simplicidade, utilidade pedagógica e continuidade.

Mais do que um ambiente técnico, a proposta é construir uma ferramenta de apoio ao ensino, capaz de aproximar o aluno de práticas reais de informática em um contexto seguro, controlado e academicamente orientado.
