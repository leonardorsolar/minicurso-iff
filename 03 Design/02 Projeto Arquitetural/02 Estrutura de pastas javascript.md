```lua
ProjetoBanco
│
├── src
│   ├── config
│   │   ├── database.js
│   │   └── env.js
│   ├── controllers
│   │   ├── AuthController.js    -- Login e Registro
│   │   └── BankController.js    -- Operações Bancárias
│   ├── models
│   │   ├── User.js              -- Usuário
│   │   ├── Account.js           -- Conta Bancária
│   │   └── Transaction.js       -- Transações
│   ├── services
│   │   ├── AuthService.js       -- Lógica de Autenticação
│   │   └── BankService.js       -- Lógica de Operações Bancárias
│   ├── routes
│   │   ├── authRoutes.js        -- Rotas de Autenticação (Login e Registro)
│   │   └── bankRoutes.js        -- Rotas de Operações Bancárias
│   ├── middleware
│   │   ├── authMiddleware.js    -- Middleware de Autenticação
│   │   └── errorHandler.js      -- Middleware de Tratamento de Erros
│   ├── utils
│   │   ├── tokenHelper.js       -- Geração e Validação de Token JWT
│   │   └── hashPassword.js      -- Função de Hashing de Senha
│   └── database
│       ├── migrations
│       │   ├── create_users_table.js
│       │   ├── create_accounts_table.js
│       │   └── create_transactions_table.js
│       └── seeds
│           └── seed_users.js
│
├── test
│   ├── controllers
│   │   ├── AuthController.test.js
│   │   └── BankController.test.js
│   └── services
│       ├── AuthService.test.js
│       └── BankService.test.js
│
├── app.js                         -- Configuração do Servidor
└── server.js                      -- Inicialização do Servidor

```
