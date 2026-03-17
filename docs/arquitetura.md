# Arquitetura do TecProfSP

## Visão geral

O **TecProfSP** foi concebido como uma **ferramenta acadêmica prática** baseada em um **servidor local de baixo custo**, destinada ao apoio das aulas técnicas de informática em escolas públicas do Estado de São Paulo.

A arquitetura proposta busca oferecer um ambiente:

- controlado;
- seguro;
- padronizado;
- de baixo custo de implantação;
- simples de manter;
- adequado ao uso didático em laboratório ou sala de aula.

O foco não está em estações individuais complexas, mas em um **servidor central local**, capaz de atender os alunos por meio de acesso web e terminal, permitindo atividades práticas de desenvolvimento, banco de dados e uso de ferramentas Linux.

---

## Conceito da arquitetura

A arquitetura do TecProfSP é baseada em um modelo de **servidor centralizado**, no qual um único equipamento hospeda o ambiente acadêmico utilizado por professores e alunos.

Esse servidor executa, em **modo texto**, todos os serviços necessários para a atividade pedagógica, disponibilizando aos usuários:

- autenticação individual;
- interface web para acesso ao ambiente;
- terminal remoto associado ao usuário;
- ferramentas de programação;
- bancos de dados para treino;
- acesso ao conteúdo didático preparado pelo professor.

Essa proposta reduz a complexidade dos equipamentos cliente e concentra a administração em um único ponto.

---

## Estrutura geral da arquitetura

A arquitetura pode ser compreendida em camadas.

### 1. Camada física

Composta por um equipamento de baixo custo, como um **Raspberry Pi**, operando como servidor local dentro da escola.

Características esperadas:

- baixo consumo de energia;
- operação contínua;
- armazenamento em cartão de 32 GB ou maior;
- funcionamento sem necessidade de placa gráfica dedicada;
- uso em rede local da escola.

---

### 2. Camada de sistema operacional

O servidor utiliza um sistema **Linux em modo texto**, sem interface gráfica.

Essa decisão arquitetural tem como finalidade:

- economizar recursos de hardware;
- aumentar estabilidade;
- simplificar manutenção;
- aproximar o aluno de ambientes profissionais reais;
- priorizar ferramentas de terminal e desenvolvimento.

---

### 3. Camada de serviços principais

Sobre o sistema operacional ficam os serviços que sustentam o ambiente acadêmico.

#### Serviços previstos

- **Apache** para publicação da interface web;
- **PHP** para construção da interface administrativa e acadêmica;
- **SSH** para acesso remoto via terminal;
- **MySQL** e **PostgreSQL** para treinamento em banco de dados;
- **Python**, **Bash** e **GCC** para atividades de programação;
- bibliotecas e dependências necessárias ao conteúdo das aulas;
- integração com **Moodle** para acesso a aulas práticas e materiais preparados pelo professor.

---

### 4. Camada de usuários

A arquitetura prevê múltiplos perfis de acesso.

#### Aluno
- acesso à interface web;
- acesso ao terminal vinculado à própria conta;
- uso de ferramentas acadêmicas liberadas;
- acesso às tarefas propostas;
- acesso ao Moodle.

#### Professor
- gerenciamento de atividades didáticas;
- organização de aulas e tarefas;
- acompanhamento do uso pelos alunos;
- apoio ao uso pedagógico do ambiente.

#### Administrador
- manutenção técnica do servidor;
- gerenciamento de serviços;
- configuração de usuários e permissões;
- atualização do ambiente.

---

## Fluxo de uso no ambiente escolar

De forma simplificada, o funcionamento da arquitetura ocorre assim:

1. O professor prepara o conteúdo e as tarefas.
2. O servidor local disponibiliza esse conteúdo aos alunos.
3. O aluno acessa a interface web usando sua conta.
4. Pela interface, o aluno visualiza tarefas e abre seu ambiente de trabalho.
5. O aluno utiliza um terminal no navegador, conectado via SSH à sua própria conta.
6. O aluno executa atividades práticas com Linux, Python, Bash, GCC, MySQL ou PostgreSQL.
7. O professor pode complementar a atividade com material disponibilizado no Moodle.

Esse modelo favorece a prática, sem exigir que cada máquina do laboratório possua configuração complexa.

---

## Componentes principais da arquitetura

## Servidor local
É o núcleo do ambiente. Centraliza autenticação, serviços, conteúdo e ferramentas.

## Interface web
Permite acesso simplificado ao ambiente, reduzindo a barreira de entrada para o aluno.

## Terminal remoto no navegador
Entrega experiência prática real de uso de Linux e desenvolvimento, sem depender de configuração local complexa no computador do aluno.

## Banco de dados individual ou controlado
Permite exercícios de modelagem, SQL e prática de estruturação de dados.

## Ambiente de aulas
O conteúdo preparado pelo professor pode ser organizado de forma padronizada, com acesso facilitado.

---

## Vantagens da arquitetura para uma escola pública em São Paulo

## 1. Baixo custo de implantação
Uma das maiores vantagens é o uso de **hardware acessível**, reduzindo o investimento inicial da escola.

Isso é importante para a rede pública, onde muitas vezes há limitação orçamentária para montagem de laboratórios completos ou aquisição de máquinas mais robustas.

---

## 2. Melhor aproveitamento de recursos
Ao centralizar o ambiente em um servidor local, a escola evita a necessidade de instalar e manter individualmente várias ferramentas em cada equipamento cliente.

Isso gera:

- menos retrabalho técnico;
- menor custo de manutenção;
- mais padronização;
- maior previsibilidade do ambiente didático.

---

## 3. Ambiente padronizado para todas as turmas
Todos os alunos utilizam o mesmo ambiente, com as mesmas ferramentas, versões e configurações.

Isso ajuda o professor a:

- preparar aulas mais consistentes;
- reduzir problemas de compatibilidade;
- facilitar suporte durante a aula;
- garantir igualdade de acesso ao conteúdo prático.

---

## 4. Segurança e controle
Por ser um ambiente controlado, a escola consegue definir:

- quem acessa;
- quais ferramentas podem ser usadas;
- quais permissões cada perfil possui;
- como os dados serão organizados.

Essa característica é especialmente importante em contexto escolar, pois reduz riscos de uso indevido, perda de configuração e exposição desnecessária do sistema.

---

## 5. Facilidade para o aluno
O aluno recebe um ambiente já preparado, com ferramentas prontas para uso.

Isso evita dificuldades comuns como:

- instalação de programas;
- configuração de dependências;
- incompatibilidades entre máquinas;
- erros iniciais de ambiente.

Na prática, o estudante pode focar mais no aprendizado e menos na preparação técnica do sistema.

---

## 6. Apoio real às disciplinas técnicas
A arquitetura atende diretamente disciplinas de informática, especialmente:

- Linux;
- Programação Python;
- Scripts Bash;
- Compilação com GCC;
- Modelagem de Dados;
- SQL com MySQL e PostgreSQL.

Ou seja, trata-se de uma arquitetura com aplicação pedagógica concreta e imediata.

---

## 7. Facilidade de renovação anual
Como o ambiente pode ser recriado a cada ano letivo, a escola consegue:

- limpar dados antigos;
- atualizar ferramentas;
- reorganizar turmas;
- reiniciar o ambiente para novas turmas;
- manter o projeto sustentável ao longo do tempo.

Isso é muito útil no contexto escolar, em que o ciclo letivo exige reorganização frequente.

---

## 8. Aproximação com o mundo profissional
Mesmo sendo uma ferramenta acadêmica, a arquitetura aproxima o aluno de práticas reais de mercado, como:

- uso de Linux em modo texto;
- acesso remoto via SSH;
- uso de servidores web;
- banco de dados relacionais;
- desenvolvimento com linguagens e compiladores reais.

Esse contato prático fortalece a formação profissional do estudante.

---

## 9. Facilidade de replicação na rede pública
Por ser uma arquitetura simples, padronizada e baseada em software amplamente conhecido, o modelo pode ser replicado em outras escolas públicas com maior facilidade.

Isso favorece:

- expansão do projeto;
- padronização entre unidades;
- compartilhamento de material didático;
- reaproveitamento de conhecimento técnico entre professores.

---

## 10. Compatibilidade com a realidade da escola pública
A arquitetura foi pensada para respeitar limitações comuns da escola pública, como:

- orçamento reduzido;
- necessidade de manutenção simplificada;
- número elevado de alunos por turma;
- demanda por ambiente seguro e controlado;
- necessidade de ferramenta prática para apoio ao professor.

Por isso, ela se encaixa bem na realidade de escolas públicas do Estado de São Paulo.

---

## Resumo da arquitetura

O **TecProfSP** adota uma arquitetura de **servidor local de baixo custo**, baseada em Linux em modo texto, com acesso web e terminal, voltada ao ensino técnico de informática.

Seu diferencial está em reunir, em um único ambiente:

- controle de acesso;
- ferramentas de desenvolvimento;
- bancos de dados para treino;
- apoio didático ao professor;
- acesso simplificado para o aluno;
- baixo custo de implantação e manutenção.

Essa arquitetura oferece uma solução prática, escalável e adequada para escolas públicas, especialmente por combinar **baixo custo**, **padronização**, **segurança**, **facilidade de uso** e **forte valor pedagógico**.
