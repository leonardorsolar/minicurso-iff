# Gerenciamento da Sprint Sprint 3

**cgatGpt:** transforme as histórias de usuários e cenários de teste em tarefas menores e liste-as em checklist no formato markdown [ ] para o arquivo .md:

## Checklist de Tarefas

### Gerenciamento de Conta (US005.1, US005.2)

-   [ ] Criar rota para visualizar informações da conta, incluindo saldo e detalhes pessoais.
-   [ ] Implementar funcionalidade para visualizar o saldo bancário atual.
-   [ ] Criar funcionalidades de depósito:
    -   [ ] Criar página de depósito.
    -   [ ] Implementar lógica para adicionar o valor ao saldo.
    -   [ ] Exibir mensagem de confirmação de depósito bem-sucedido.
    -   [ ] Implementar validação de valor inválido (negativo ou zero).
-   [ ] Criar funcionalidades de saque:
    -   [ ] Criar página de saque.
    -   [ ] Implementar lógica para subtrair o valor do saldo.
    -   [ ] Exibir mensagem de confirmação de saque bem-sucedido.
    -   [ ] Implementar validação de valor inválido (negativo ou zero).
    -   [ ] Implementar validação de saldo insuficiente.

### Histórico de Transações (US006.1, US006.2)

-   [ ] Criar rota para visualizar o histórico de transações.
-   [ ] Implementar funcionalidade para listar todas as transações, incluindo depósitos e saques.
-   [ ] Implementar lógica para filtragem por data:
    -   [ ] Adicionar interface para seleção de intervalo de datas.
    -   [ ] Implementar lógica para mostrar transações dentro do intervalo selecionado.
-   [ ] Implementar lógica para filtragem por tipo de transação (depósito ou saque):
    -   [ ] Adicionar interface para seleção do tipo de transação.
    -   [ ] Implementar lógica para mostrar transações do tipo selecionado.
-   [ ] Implementar tratamento para histórico vazio:
    -   [ ] Exibir mensagem informando que não há transações para exibir quando o histórico estiver vazio.
-   [ ] Implementar tratamento para filtragem sem resultados:
    -   [ ] Exibir mensagem informando que não há transações que correspondem aos critérios de filtragem.
