## Sprint 2.2: Consulta de Saldo e Histórico de Transações

        Duração: 2 semanas (16/10/2024 - 30/10/2024)
        Objetivos:
            Implementar funcionalidades de consulta de saldo e visualização de histórico de transações.
        Backlog:
            US002.2.1: Implementar consulta de saldo da conta.
            US002.2.1: Implementar visualização do histórico de transações.

**cgatGpt:** transforme as funcionalidades a seguir em histórias de usuários e cenários de teste de aceitação do tipo Give, when, then:

# Histórias de Usuário e Cenários de Teste

História de Usuário e Cenários de Teste
US002.2.1: Implementar consulta de saldo da conta

História de Usuário: Como usuário, desejo consultar o saldo da minha conta para acompanhar meu saldo disponível em tempo real.

Cenários de Teste de Aceitação:

    Cenário: Consulta de saldo bem-sucedida
        Dado que o usuário está autenticado e na página de consulta de saldo,
        Quando ele solicita a visualização do saldo,
        Então ele deve ver o saldo atual da sua conta exibido na página.

    Cenário: Falha na consulta de saldo
        Dado que o usuário está autenticado e na página de consulta de saldo,
        Quando ocorre uma falha na comunicação com o servidor,
        Então ele deve ver uma mensagem de erro informando que a consulta de saldo não pôde ser realizada.

    Cenário: Acesso à página de saldo sem autenticação
        Dado que o usuário não está autenticado e tenta acessar a página de consulta de saldo,
        Quando ele tenta acessar a página de saldo,
        Então ele deve ser redirecionado para a página de login com uma mensagem informando que a autenticação é necessária.

US002.2.2: Implementar visualização do histórico de transações

História de Usuário: Como usuário, desejo visualizar o histórico de transações da minha conta para acompanhar minhas despesas e receitas.

Cenários de Teste de Aceitação:

    Cenário: Visualização do histórico de transações bem-sucedida
        Dado que o usuário está autenticado e na página de histórico de transações,
        Quando ele solicita a visualização do histórico de transações,
        Então ele deve ver uma lista detalhada das transações realizadas, incluindo data, valor e descrição.

    Cenário: Falha na visualização do histórico de transações
        Dado que o usuário está autenticado e na página de histórico de transações,
        Quando ocorre uma falha na comunicação com o servidor,
        Então ele deve ver uma mensagem de erro informando que a visualização do histórico de transações não pôde ser realizada.

    Cenário: Acesso ao histórico de transações sem autenticação
        Dado que o usuário não está autenticado e tenta acessar a página de histórico de transações,
        Quando ele tenta acessar a página de histórico de transações,
        Então ele deve ser redirecionado para a página de login com uma mensagem informando que a autenticação é necessária.

# Gerenciamento da Sprint Sprint 2.2

**cgatGpt:** transforme as histórias de usuários e cenários de teste em tarefas menores e liste-as em checklist no formato markdown [ ] para ser acionado no arquivo .md :

## Checklist de Tarefas

### US002.2.1: Implementar consulta de saldo da conta

-   [ ] **Criar a página de consulta de saldo**

    -   [ ] Adicionar campo para exibição do saldo.
    -   [ ] Adicionar lógica para autenticação do usuário.

-   [ ] **Implementar a lógica de consulta de saldo**

    -   [ ] Desenvolver API para recuperar o saldo da conta.
    -   [ ] Integrar a API com a página de consulta de saldo.

-   [ ] **Tratar erros de comunicação**

    -   [ ] Implementar tratamento de falhas na comunicação com o servidor.
    -   [ ] Exibir mensagem de erro caso a consulta de saldo falhe.

-   [ ] **Implementar redirecionamento para a página de login**

    -   [ ] Verificar a autenticação do usuário ao acessar a página de saldo.
    -   [ ] Redirecionar usuários não autenticados para a página de login com mensagem informativa.

-   [ ] **Criar testes automatizados**
    -   [ ] **Cenário: Consulta de saldo bem-sucedida**
        -   [ ] Dado que o usuário está autenticado e na página de consulta de saldo,
        -   [ ] Quando ele solicita a visualização do saldo,
        -   [ ] Então ele deve ver o saldo atual da sua conta exibido na página.
    -   [ ] **Cenário: Falha na consulta de saldo**
        -   [ ] Dado que o usuário está autenticado e na página de consulta de saldo,
        -   [ ] Quando ocorre uma falha na comunicação com o servidor,
        -   [ ] Então ele deve ver uma mensagem de erro informando que a consulta de saldo não pôde ser realizada.
    -   [ ] **Cenário: Acesso à página de saldo sem autenticação**
        -   [ ] Dado que o usuário não está autenticado e tenta acessar a página de consulta de saldo,
        -   [ ] Quando ele tenta acessar a página de saldo,
        -   [ ] Então ele deve ser redirecionado para a página de login com uma mensagem informando que a autenticação é necessária.

---

### US002.2.2: Implementar visualização do histórico de transações

-   [ ] **Criar a página de histórico de transações**

    -   [ ] Adicionar campo para exibição do histórico de transações.
    -   [ ] Adicionar lógica para autenticação do usuário.

-   [ ] **Implementar a lógica de visualização do histórico de transações**

    -   [ ] Desenvolver API para recuperar o histórico de transações.
    -   [ ] Integrar a API com a página de histórico de transações.

-   [ ] **Tratar erros de comunicação**

    -   [ ] Implementar tratamento de falhas na comunicação com o servidor.
    -   [ ] Exibir mensagem de erro caso a visualização do histórico de transações falhe.

-   [ ] **Implementar redirecionamento para a página de login**

    -   [ ] Verificar a autenticação do usuário ao acessar a página de histórico de transações.
    -   [ ] Redirecionar usuários não autenticados para a página de login com mensagem informativa.

-   [ ] **Criar testes automatizados**
    -   [ ] **Cenário: Visualização do histórico de transações bem-sucedida**
        -   [ ] Dado que o usuário está autenticado e na página de histórico de transações,
        -   [ ] Quando ele solicita a visualização do histórico de transações,
        -   [ ] Então ele deve ver uma lista detalhada das transações realizadas, incluindo data, valor e descrição.
    -   [ ] **Cenário: Falha na visualização do histórico de transações**
        -   [ ] Dado que o usuário está autenticado e na página de histórico de transações,
        -   [ ] Quando ocorre uma falha na comunicação com o servidor,
        -   [ ] Então ele deve ver uma mensagem de erro informando que a visualização do histórico de transações não pôde ser realizada.
    -   [ ] **Cenário: Acesso ao histórico de transações sem autenticação**
        -   [ ] Dado que o usuário não está autenticado e tenta acessar a página de histórico de transações,
        -   [ ] Quando ele tenta acessar a página de histórico de transações,
        -   [ ] Então ele deve ser redirecionado para a página de login com uma mensagem informando que a autenticação é necessária.
