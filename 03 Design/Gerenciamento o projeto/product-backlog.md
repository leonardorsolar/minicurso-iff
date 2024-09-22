# Product Backlog - histórias de usuários

Product Backlog: Lista de funcionalidades (histórias de usuários) que devem ser implementadas no sistema.

## Product Backlog

## 1 - Registro de Usuário

US001.1: Como um usuário, quero me registrar na plataforma para poder acessar minha conta bancária.
US001.2: O sistema deve verificar se o e-mail já está registrado e retornar uma mensagem de erro se houver duplicação.

## 2 - Login de Usuário

US002.1: Como um usuário, quero fazer login na plataforma para acessar minha conta.
US002.2: Após a autenticação, a API deve gerar um token JWT para permitir o acesso a rotas protegidas.

## 3 - Autenticação e Autorização

US003.1: A API deve validar tokens JWT para todas as requisições a rotas protegidas.
US003.2: Deve haver controle de permissões para que apenas usuários autenticados possam acessar seus próprios dados.

## 4 - Recuperação de Senha

US004.1: Como um usuário, quero solicitar um link de redefinição de senha para recuperar o acesso à minha conta.
US004.2: A API deve permitir que o usuário defina uma nova senha por meio de um token temporário enviado por e-mail.

## 5 - Gerenciamento de Conta

US005.1: Como um usuário, quero visualizar as informações da minha conta, incluindo saldo e detalhes pessoais.
US005.2: Como um usuário, quero visualizar as opções de depósito, saque e transferência ao acessar a página de saldo.

## 6 - Histórico de Transações

US006.1: Como um usuário, quero visualizar meu histórico de transações (depósitos, saques e transferências).
US006.2: O sistema deve permitir filtrar transações por data e tipo.

## 7 - Transações Bancárias

US007.1: Como um usuário, quero fazer transferências para outras contas, fornecendo a conta de destino e o valor.
US007.2: O sistema deve garantir que o saldo seja atualizado corretamente após cada transação.
US007.3: O sistema deve impedir transações que deixem o saldo negativo.

## 8 - Logout

US008.1: Como um usuário, quero encerrar minha sessão para que ninguém mais tenha acesso à minha conta.

obs.:
o formato US001.1 indica a primeira história relacionada à funcionalidade de Registro de Usuário, enquanto US001.2 indica um requisito adicional ou uma condição dentro da mesma funcionalidade.
