# Gerenciamento da Qualidade do Projeto - Conta Bancária

## Introdução

Este documento descreve o gerenciamento da qualidade para o projeto de conta bancária com funcionalidades de login e registro do usuário. O objetivo é garantir que o sistema atenda aos requisitos e padrões de qualidade estabelecidos.

## 1. Objetivos de Qualidade

### 1.1 Objetivo do Projeto

Desenvolver uma aplicação bancária que permita aos usuários se registrar, fazer login e gerenciar suas contas com segurança e eficiência.

### 1.2 Objetivos de Qualidade

-   Garantir que as funcionalidades de login e registro funcionem corretamente e sem falhas.
-   Assegurar que o sistema seja seguro e que os dados do usuário sejam protegidos.
-   Validar que a interface do usuário seja intuitiva e fácil de usar.
-   Confirmar que o sistema seja confiável e eficiente.

## 2. Estratégia de Teste

### 2.1 Tipos de Testes

-   **Testes Funcionais:** Verificam se as funcionalidades do sistema atendem aos requisitos especificados.
-   **Testes de Usabilidade:** Avaliam a facilidade de uso e a experiência do usuário.
-   **Testes de Segurança:** Garantem que os dados dos usuários estejam protegidos contra acesso não autorizado.
-   **Testes de Desempenho:** Medem a eficiência e a velocidade do sistema.
-   **Testes de Compatibilidade:** Asseguram que o sistema funcione em diferentes navegadores e dispositivos.

### 2.2 Ferramentas de Teste

-   **Automatização:** Jest, Mocha
-   **Segurança:** OWASP ZAP
-   **Desempenho:** JMeter
-   **Usabilidade:** Testes manuais e feedback de usuários

### 3.1 Critérios de Aceitação

#### Registro de Usuário

-   **Critério 1:** O usuário deve ser capaz de se registrar com um e-mail e senha válidos.
-   **Critério 2:** O sistema deve verificar se o e-mail já está em uso e informar o usuário adequadamente.
-   **Critério 3:** Após o registro, o usuário deve receber um e-mail de verificação.

#### Login

-   **Critério 1:** O usuário deve conseguir fazer login com e-mail e senha válidos.
-   **Critério 2:** O sistema deve solicitar autenticação de dois fatores se ativada.
-   **Critério 3:** O sistema deve fornecer mensagens de erro apropriadas para credenciais incorretas.

#### Funcionalidades Adicionais

-   **Critério 1:** O usuário deve conseguir consultar o saldo da conta.
-   **Critério 2:** O usuário deve poder visualizar o histórico de transações de forma detalhada.

### 3.2 Plano de Testes

#### Testes de Funcionalidade

-   **Registro de Usuário**

    -   **Cenário:** Registro bem-sucedido
        -   **Dado que** o usuário está na página de registro,
        -   **Quando** ele preenche os campos de e-mail e senha e clica no botão de registrar,
        -   **Então** ele deve receber uma confirmação de que a conta foi criada com sucesso.
    -   **Cenário:** Registro com e-mail já em uso
        -   **Dado que** o usuário tenta registrar um e-mail já existente,
        -   **Quando** ele clica em registrar,
        -   **Então** ele deve ver uma mensagem informando que o e-mail já está em uso.

-   **Login**

    -   **Cenário:** Login bem-sucedido
        -   **Dado que** o usuário está na página de login,
        -   **Quando** ele insere um e-mail e senha válidos e clica no botão de login,
        -   **Então** ele deve ser redirecionado para a página principal da conta.
    -   **Cenário:** Login com credenciais incorretas
        -   **Dado que** o usuário insere e-mail ou senha incorretos,
        -   **Quando** ele tenta fazer login,
        -   **Então** ele deve ver uma mensagem de erro informando que as credenciais estão incorretas.

-   **Consulta de Saldo e Histórico de Transações**
    -   **Cenário:** Consulta de saldo bem-sucedida
        -   **Dado que** o usuário está autenticado,
        -   **Quando** ele solicita a visualização do saldo,
        -   **Então** o saldo atual deve ser exibido na página.
    -   **Cenário:** Visualização do histórico de transações
        -   **Dado que** o usuário está autenticado,
        -   **Quando** ele solicita o histórico de transações,
        -   **Então** ele deve ver uma lista detalhada das transações realizadas.

## 4. Garantia da Qualidade

### 4.1 Revisão de Código

-   **Revisores:** Todo código deve ser revisado por pelo menos um membro da equipe antes de ser mesclado na branch principal.
-   **Critérios de Revisão:** Verificar a aderência aos requisitos, padrões de codificação e a ausência de bugs.

### 4.2 Gestão de Defeitos

-   **Registro de Defeitos:** Todos os defeitos encontrados devem ser registrados em um sistema de rastreamento de defeitos (ex.: Jira).
-   **Resolução de Defeitos:** Defeitos devem ser priorizados e corrigidos com base em sua gravidade e impacto.

### 4.3 Melhoria Contínua

-   **Feedback:** Coletar feedback dos usuários para identificar áreas de melhoria.
-   **Atualizações:** Revisar e atualizar processos e práticas de qualidade regularmente para garantir que permaneçam eficazes.

### 4.4 Métricas de Avaliação

#### 4.4.1 Métricas de Desempenho

-   **Tempo de Resposta:** Medir o tempo que o sistema leva para processar e responder a solicitações do usuário.
-   **Taxa de Erros:** Percentual de erros encontrados durante o uso normal do sistema.

#### 4.4.2 Métricas de Funcionalidade

-   **Taxa de Sucesso de Testes:** Percentual de cenários de teste bem-sucedidos em relação ao total de testes executados.
-   **Número de Defeitos:** Quantidade de defeitos encontrados em cada fase do ciclo de vida do projeto.

#### 4.4.3 Métricas de Usabilidade

-   **Satisfação do Usuário:** Avaliações e feedback dos usuários sobre a facilidade de uso do sistema.
-   **Tempo de Aprendizado:** Tempo médio necessário para que novos usuários se familiarizem com o sistema.

#### 4.4.4 Métricas de Segurança

-   **Número de Vulnerabilidades:** Quantidade de vulnerabilidades identificadas durante os testes de segurança.
-   **Tempo para Correção:** Tempo médio necessário para corrigir vulnerabilidades de segurança.

### 4.6 Padrões de Semântica de Commit

#### 4.6.1 Padrões de Commit

-   **Commit Mensagens:** Seguir o padrão de commit "Conventional Commits" para garantir clareza e consistência.
    -   **Formato:** `<tipo>(<escopo>): <descrição>`
    -   **Tipos Comuns:** feat (nova funcionalidade), fix (correção de bug), docs (documentação), style (estilo de código), refactor (refatoração de código), test (testes), chore (tarefas gerais).
-   **Exemplo:** `feat(auth): adicionar autenticação de dois fatores`
-   \*\*Objetivo:\*\* Facilitar a leitura do histórico de commits e melhorar a integração com ferramentas de automação e versionamento.

## 5. Documentação de Qualidade

### 5.1 Relatórios de Testes

-   **Relatórios:** Gerar relatórios de testes detalhados após a execução dos testes, incluindo os resultados e quaisquer defeitos encontrados.

### 5.2 Documentação de Procedimentos

-   **Procedimentos:** Documentar todos os procedimentos de teste e controle de qualidade, incluindo critérios de aceitação e planos de teste.

## 6. Contatos

### 6.1 Equipe de Qualidade

-   **Líder de Qualidade:** Nome, e-mail
-   **Especialistas em Testes:** Nome, e-mail

### 6.2 Suporte

-   **E-mail de Suporte:** suporte@empresa.com
