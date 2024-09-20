# Análise

## Requisitos Funcionais:

# 1-Registro de Usuário:

A API deve permitir a criação de novos usuários enviando informações como nome, e-mail, senha e confirmação de senha.
O sistema deve verificar se o e-mail já está registrado e retornar uma mensagem de erro apropriada se houver duplicação.

# 2-Login de Usuário:

A API deve permitir que usuários façam login enviando e-mail e senha.
Após a autenticação bem-sucedida, a API deve gerar um token JWT (ou outro mecanismo de autenticação) para permitir o acesso a rotas protegidas.

# 3-Autenticação e Autorização:

A API deve validar tokens JWT para todas as requisições a rotas protegidas.
Deve haver controle de permissões, garantindo que apenas usuários autenticados possam acessar seus próprios dados.

# 4-Recuperação de Senha:

A API deve fornecer uma rota para enviar um link de redefinição de senha para o e-mail do usuário.
A API deve permitir que o usuário defina uma nova senha por meio de um token temporário enviado por e-mail.

# 5-Gerenciamento de Conta:

A API deve permitir que o usuário visualize as informações de sua conta, incluindo saldo e detalhes pessoais.
A API deve permitir que o usuário edite suas informações, como nome e senha.

# 6-Histórico de Transações:

A API deve fornecer uma rota para que o usuário visualize o histórico de transações (depósitos, saques e transferências).
Deve haver suporte para filtrar transações por data e tipo.

# 7-Transações Bancárias:

A API deve permitir que o usuário faça transferências para outras contas, fornecendo a conta de destino e o valor.
Deve garantir que o saldo seja atualizado corretamente após cada transação e que não seja possível realizar transações que deixem o saldo negativo.

# 8-Logout:

A API deve permitir que o usuário encerre sua sessão invalidando o token de autenticação.
