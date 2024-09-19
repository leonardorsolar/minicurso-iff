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

No vscode: Instale a estensão Draw.io Integration no vscode

Na web: utilize um dos aplicativos a seguir:
https://app.diagrams.net/
https://miro.com/pt/

## Passo 3: Crie o arquivo Event Storming Bank Account.drawio e salve na pasta 01 EventStorming

Event Storming Bank Account.drawio

## Passo 4: Iniciando a seção do Event Storming

Prática na sala de aula:

Pergunta: Quais são os eventos existem na sequência do fluxo do processo para cada usuário?
Pergunta: quais novos eventos deveriam existir no processo.

# Mapear Eventos

## Eventos (Domain event)

[Sujeito] [Verbo]
Representação: sticky notes Laranja.

## Parte 4.1: Crie os eventos de cada usuário do sistema numa linha vertical

(ações, interações com usuários ou software)

Ator (User)
Representação: pequeno sticky notes Amarelo.

**cgatGpt:** Vamos utilizar o Event Storming. Evento (Domain event): os eventos são conjugados no passado, por exemplo: Cadastro Criado, Pagamento Criado. Assim crie o event storming para o cliente do banco, ordenado os eventos numa linha do tempo de acontecimentos para um projeto back end de uma conta bancaria contendo login e registro do usuário.

Representação: sticky notes Laranja.

**cgatGpt:** Vamos utilizar o Event Storming. Evento (Domain event): os eventos são conjugados no passado, por exemplo: Cadastro Criado, Pagamento Criado. Assim crie o event storming para o acesso do gerente do banco, ordenado os eventos numa linha do tempo de acontecimentos para um projeto back end de uma conta bancaria contendo login e registro do usuário.

## Parte 4.3: Adicionar eventos que são gerados automaticamente, disprados pelo tempo, após o cumprimento de condições temporais.

Pergunte ao time se existe algum evento que é disparado sem nenhum usuário ou sistema envolvido?
Uma ferrementa de notificação, de agendamento, do banco de dados...

**cgatGpt:** (Eventos - Domain event) cite eventos,conjugados no passado, que são disparados pelo tempo e não por ações, interações com usuários ou software, por exemplo: Proposta pendente há mais de 10 dias”? Esse eventos desem no passado para o projeto back end de uma conta bancaria contendo login e registro do usuário

# Linha do tempo

## Parte 4.4: coloque os eventos de forma ordenada numa linha do tempo de acontecimentos (hotizontal)

Pergunta: quais novos eventos deveriam existir no processo?

À medida que evoluir com os eventos, verifique se é preciso reordenar.

# Comandos (Command)

[Verbo][Sujeito]
Representação: sticky notes Azul claro.

## Parte 4.5: para acada evento crie um card de comando que é uma ação, interação ou decisão que leva ao evento com o qual está relacionado. Algo realizado por um usuário ou sistema externo.

Analise todos eventos que já adicionou no board
Adicione o sticky de comando ao lado esquerdo de cada evento existente
Descreva os comandos com verbos transitivos, como exemplo: Criar, Deletar, Enviar, Transacionar, etc

Pergunta: quais seriam as ações que cada usuário ou sistema que levou a ocorrer o evento
Adicione o ator que disparou o comando para esclarecer as responsabilidades.

**cgatGpt:** Comandos (Command) para acada evento crie um card de comando que é uma ação ,nteração ou decisão que leva ao evento com o qual está relacionado. Algo realizado por um usuário ou sistema externo. Descreva os comandos com verbos transitivos, como exemplo: Criar, Deletar, Enviar, Transacionar, etc; para projeto back end de uma conta bancaria contendo login e registro do usuário

## Questões (Concern)

[Sujeito] [Verbo]
Representação: sticky notes Rosa

## Parte 4.6: adicionar os cards de dúvidas existentes ou preocupações do sistema

Coloquem em ordem de prioridade as dúvidas/preocupações da esquerda para a direita.

Esclareça cada termo ou evento que gerou dúvidas

(opicional: inclua nota em forma de pergunta sobre possíveis fluxo de erros que podem ocorrer com o evento)

## Políticas (Business process)

Representação: sticky notes Roxo.

## Parte 4.7: adicionar as políticas que são os cards que indicam decições a serem tomadas, que dispararão novos comandos e eventos. (processo decisório do fluxo)

**cgatGpt:** Políticas (Business process) defina políticas existentes que indicam decições a serem tomadas, que dispararão novos comandos e eventos do projeto back end de uma conta bancaria contendo login e registro do usuário.

Quais processos decisórios são consequências de cada um dos eventos no board?
Adicione o relacionamento da política ao elemento correspondente ao ponto onde se faz necessária a decisão de negócio.

## Sistema Externo (External system)

Representação: sticky notes Rosa claro.

## Parte 4.8: adicionar dependência com algum sistema externo

Existe alguma dependência com algum sistema externo para consulta ou execução de ação/comando.

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

## Parte 4.9: procure identificar as principais entidades do sistema

Agregação (Aggregate)
Representação: sticky notes Amarelo Claro.

As agregações são grupos de entidades que são tratadas como uma única unidade para fins de consistência e transações.

1. Conecte os eventos/comandos às agregações

2. Defina o nome da agregação utilizando um substantivo que descreva os dados contidos no conjunto

3. Dentro de um boundary (vide abaixo) não deve existir duas agregações com o mesmo nome

Boundaries
Representação: Retângulo com borda preta tracejada

Os boundaries ajudam a identificar as agregações correlacionadas dentro do mesmo contexto.

**cgatGpt:** para este event storming do projeto back end de uma conta bancaria contendo login e registro do usuário, defina as Agregações (Aggregates) e os Boundaries

## Passo 5: Definindo a Arquitetura

Podemos definir a arquitetura mvc, em camadas, hexagonal, clean architeture, entre outras.

## Parte 1: Estururação das pasta de acordo com a arquitetura mvc

**cgatGpt-java:** como ficaria o estrutura das pasta e os arquivos para o java, utilizando arquitetura mvc, utilizando o formato de Markdown para o projeto back end para os móduloes bancaria, login e registro de usuários .Somente cite a estruturação das pasta em makdown

**cgatGpt-javaScript:** como ficaria o estrutura e os arquivos das pasta para o javascript, utilizando arquitetura mvc, utilizando o formato de Markdown para o projeto back end para os móduloes bancaria, login e registro de usuários .Somente cite a estruturação das pasta em makdown

Alternativa: Utilize a pasta infrastructure para o banco de dafos e serviços externos, a pasta share para arquivos compartilhados, a pasta test para os teste unitario e de integração,

## Passo 6: Definindo os diagramas

## Parte 1: Diagrama de classes

**cgatGpt:** como ficaria o diagrama de classes utilizando o formato de Markdown para o projeto back end para os móduloes bancaria, login e registro de usuários .Somente cite a estruturação das pasta em makdown

## Passo 7: Definindo o Diagrama do Banco de dados

## Parte 1: Diagrama do Banco de dados

**cgatGpt:** Para o projeto de conta bancária com login crie o diagrama do banco de dados para o projeto back end para os móduloes bancaria, login e registro de usuários .Somente cite a estruturação das pasta em makdown

## Passo 8: Definindo o Protópipo

## Parte 5: Projeto Interface - Protótipo

**cgatGpt:** Crie um código em html, css e javascript de uma tela de registro de usuário e login usando a biblioteca boostrap e fazendo um requisição do tipo post no endereço localhost:3000/api/cirarUsuario para o registro de usuário e um requisição do tipo post no endereço localhost:3000/api/auht

https://www.figma.com/

## Passo 9: Definindo itens para o gerenciamento do projeto

## Backlog do produto (Product Backlog):

**cgatGpt:** Crie o product backlog, a release plan e a sprint plan para o projeto conta bancaria que tem login e registro do usuário, utlise a notação 1 nome da funciolidade e us001.1 para historia de usuários
