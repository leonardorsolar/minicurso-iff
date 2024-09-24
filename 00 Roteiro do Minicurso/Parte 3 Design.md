# Design

## Passo 1: Crie a seguinte estutura de pastas:

```lua
Minicurso
│
├── 00 Minicurso
│ ├── ...
│    └── ...
│
├── 03 Design
│ │
│ ├── 01 EventStorming
│ │   └── 01 Event Storming Bank Account.drawio
│ │
│ ├── 02 Projeto Arquitetural
│ │   └── 01 ...
│ │   └── 02 ...
│ │
│ ├── 03 Diagramas
│ │   └── 01 ...
│ │   └── 02 ...
│ │
│ ├── 04 Projeto Banco de dados
│ │   └── 01 ...
│ │   └── 02 ...
│ │
│ ├── 05 Projeto Interface
│ │   └── 01 ...
│ │   └── 02 ...
│ │
│ ├── 06 Gerenciamento o projeto
│ │   └── 01 ...
│ │   └── 02 ...
└──
```

## Passo 2: Aplicativo de criação de diagrama

No vscode: Instale a extensão Draw.io Integration no vscode

Na web: utilize um dos aplicativos a seguir:
https://app.diagrams.net/
https://miro.com/pt/

## Passo 3: Crie o arquivo Event Storming Bank Account.drawio e salve na pasta 01 EventStorming

Event Storming Bank Account.drawio

## Passo 4: Iniciando a seção do Event Storming

# Fase 1: Mapear Eventos

## Eventos (Domain event)

[Sujeito] [Verbo]
Representação: sticky notes Laranja.

## Parte 4.1: Defina quem são os usuários do sistema

(ações, interações com usuários ou software)

Ator (User)
Representação: pequeno sticky notes Amarelo.

Prática na sala de aula:

Pergunta: Quem são os usuários do sistema?

## Parte 4.2: Crie os eventos de cada usuário do sistema numa linha vertical

Representação: sticky notes Laranja.

**cgatGpt:** Vamos utilizar o Event Storming. Evento (Domain event): os eventos são conjugados no passado, por exemplo: Cadastro Criado, Pagamento Criado. Assim crie o event storming para o acesso do gerente do banco, ordenado os eventos numa linha do tempo de acontecimentos para um projeto back end de uma conta bancaria contendo login e registro do usuário.

Prática na sala de aula:

Pergunta: Quais são os eventos existem na sequência do fluxo do processo para cada usuário?
Pergunta: quais novos eventos deveriam existir no processo.

## Parte 4.3: Adicionar eventos que são gerados automaticamente, disparados pelo tempo, após o cumprimento de condições temporais.

Prática na sala de aula:

Pergunta: Existe algum evento que é disparado sem nenhum usuário ou sistema envolvido?
Uma ferrementa de notificação, de agendamento, do banco de dados...

**cgatGpt:** (Eventos - Domain event) cite eventos,conjugados no passado, que são disparados pelo tempo e não por ações, interações com usuários ou software, por exemplo: Proposta pendente há mais de 10 dias”? Esse eventos desem no passado para o projeto back end de uma conta bancaria contendo login e registro do usuário

# Fase 2: Linha do tempo

## Parte 4.4: coloque os eventos de forma ordenada numa linha do tempo de acontecimentos (hotizontal)

Pergunta: quais novos eventos deveriam existir no processo?

À medida que evoluir com os eventos, verifique se é preciso reordenar.

## Parte 4.5: para acada evento crie um card de comando que é uma ação, interação ou decisão que leva ao evento com o qual está relacionado. Algo realizado por um usuário ou sistema externo.

# Comandos (Command)

[Verbo][Sujeito]
Representação: sticky notes Azul claro.

Analise todos eventos que já adicionou no board
Adicione o sticky de comando ao lado esquerdo de cada evento existente
Descreva os comandos com verbos transitivos, como exemplo: Criar, Deletar, Enviar, Transacionar, etc

Pergunta: quais seriam as ações que cada usuário ou sistema que levou a ocorrer o evento
Adicione o ator que disparou o comando para esclarecer as responsabilidades.

**cgatGpt:** Comandos (Command) para acada evento crie um card de comando que é uma ação ,nteração ou decisão que leva ao evento com o qual está relacionado. Algo realizado por um usuário ou sistema externo. Descreva os comandos com verbos transitivos, como exemplo: Criar, Deletar, Enviar, Transacionar, etc; para projeto back end de uma conta bancaria contendo login e registro do usuário

## Parte 4.6: adicionar os cards de dúvidas existentes ou preocupações do sistema

## Questões (Concern)

[Sujeito] [Verbo]
Representação: sticky notes Rosa

Coloquem em ordem de prioridade as dúvidas/preocupações da esquerda para a direita, abaixo dos comando e eventos.

Esclareça cada termo ou evento que gerou dúvidas, anote-os

(opicional: inclua nota em forma de pergunta sobre possíveis fluxo de erros que podem ocorrer com o evento)

## Parte 4.7: adicionar as políticas que são os cards que indicam decições a serem tomadas, que dispararão novos comandos e eventos. (processo decisório do fluxo)

## Políticas (Business process)

Representação: sticky notes Roxo.

**cgatGpt:** Políticas (Business process) defina políticas existentes que indicam decições a serem tomadas, que dispararão novos comandos e eventos do projeto back end de uma conta bancaria contendo login e registro do usuário.

Quais processos decisórios são consequências de cada um dos eventos no board?
Adicione o relacionamento da política ao elemento correspondente ao ponto onde se faz necessária a decisão de negócio.

## Parte 4.8: adicionar dependência com algum sistema externo

## Sistema Externo (External system)

Representação: sticky notes Rosa claro.

Pergunta: Existe alguma dependência com algum sistema externo para consulta ou execução de ação/comando.

**cgatGpt:** para este event storming do projeto back end de uma conta bancaria contendo login e registro do usuário, defina quais são as dependêcias com sistemas externos que podem gerar ação ou comando no sistema.

## Parte 4.9: adicionar pontos do sistema onde é necessário dispor de uma interface para consulta de informações

## Modo Leitura (View)

Representação: sticky notes Verde Claro.

**cgatGpt:** para este event storming do projeto back end de uma conta bancaria contendo login e registro do usuário, identifique todos os pontos do sistema onde é necessário dispor de uma interface para consulta de informações. seja tela para consulta, um local de relatórios, push notifificação, consulta sql ou outra

Qual local existe/existirá alguma:

-   tela para consulta
-   um local de relatórios
-   push notifificação
-   consulta sql

# Fase 3: Análise

## Parte 4.9: procure identificar as principais entidades do sistema

## Agregação (Aggregate)

Representação: sticky notes Amarelo Claro.

As agregações são grupos de entidades que são tratadas como uma única unidade para fins de consistência e transações.

1. Conecte os eventos/comandos às agregações

2. Defina o nome da agregação utilizando um substantivo que descreva os dados contidos no conjunto

3. Dentro de um boundary (vide abaixo) não deve existir duas agregações com o mesmo nome

## Boundaries

Representação: Retângulo com borda preta tracejada

Os boundaries ajudam a identificar as agregações correlacionadas dentro do mesmo contexto.

**cgatGpt:** para este event storming do projeto back end de uma conta bancaria contendo login e registro do usuário, defina as Agregações (Aggregates) e os Boundaries

## Passo 4: Definindo a Arquitetura

Podemos definir a arquitetura mvc, em camadas, hexagonal, clean architeture, entre outras.

## Parte 1: Estruturação das pasta de acordo com a arquitetura mvc

**cgatGpt-java:** como ficaria o estrutura das pasta e os arquivos para o java, utilizando arquitetura mvc, utilizando o formato de Markdown para o projeto back end para os móduloes bancaria, login e registro de usuários .Somente cite a estruturação das pasta em markdown.lua. Ex.: `lua ... `

**cgatGpt-javaScript:** como ficaria o estrutura e os arquivos das pasta para o javascript, utilizando arquitetura mvc, utilizando o formato de Markdown para o projeto back end para os módulos bancário, login e registro de usuários. Somente cite a estruturação das pasta em markdown.lua

Alternativa: Utilize a pasta infrastructure para o banco de dafos e serviços externos, a pasta share para arquivos compartilhados, a pasta test para os teste unitario e de integração,

## Passo 5: Definindo os diagramas

## Parte 1: Diagrama de classes

**cgatGpt:** como ficaria o diagrama de classes utilizando o formato de Markdown para o projeto back end para os móduloes bancaria, login e registro de usuários para uma arquitetura mvc simples.

## Passo 6: Definindo o Diagrama do Banco de dados

## Parte 1: Diagrama do Banco de dados

**cgatGpt:** Para o projeto de conta bancária com login crie o diagrama do banco de dados para o projeto back end para os módulos bancários, login e registro de usuários.

## Passo 7: Definindo o Protópipo

## Parte 1: Projeto Interface - Protótipo

**cgatGpt:** Crie 2 páginas com o código em html, css e javascript, sendo uma paǵina seria a de registro de usuário fazendo um requisição do tipo post no endereço localhost:3000/api/cirarUsuario e a outra página de login usando a biblioteca boostrap com uma requisição do tipo post no endereço localhost:3000/api/auht. A de login tem um link regitre-se que chama a tela de registro e a de registro tem um link para voltar na tela de login. Coloque-o formulário de forma centralizanda e reponsiva.

Abra o vscode, crie os arquivos e cole o código.

Outra opção seria criar um protótipo no porgrama figma: (vantagem de mais fidelidade no design)
https://www.figma.com/

## Passo 8: Definindo itens para o gerenciamento do projeto

## Parte 1: Backlog do produto (Product Backlog):

**cgatGpt:** Crie o product backlog, a release plan e a sprint plan para o projeto back end conta bancaria que tem login e registro do usuário, utilizando a notação 1 nome da funciolidade e us001.1 para historia de usuários. Utilize somente as funcionalidade do back end e se necessário inclua mais funcionalidades: "cole as funcionalidades do arquivo 02 Análise/02 Back/Requisitos funcionais.md aqui."
