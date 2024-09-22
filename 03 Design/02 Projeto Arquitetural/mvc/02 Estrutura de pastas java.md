````lua
ProjetoBanco
│
├── src
│   ├── main
│   │   ├── java
│   │   │   ├── config
│   │   │   │   ├── DatabaseConfig.java
│   │   │   │   └── SecurityConfig.java
│   │   │   ├── controllers
│   │   │   │   ├── AuthController.java   -- Login e Registro
│   │   │   │   └── BankController.java   -- Operações Bancárias
│   │   │   ├── models
│   │   │   │   ├── User.java
│   │   │   │   ├── Account.java
│   │   │   │   └── Transaction.java
│   │   │   ├── services
│   │   │   │   ├── AuthService.java      -- Lógica de Autenticação
│   │   │   │   └── BankService.java      -- Lógica de Transações Bancárias
│   │   │   ├── repositories
│   │   │   │   ├── UserRepository.java
│   │   │   │   ├── AccountRepository.java
│   │   │   │   └── TransactionRepository.java
│   │   │   ├── security
│   │   │   │   ├── JwtUtil.java
│   │   │   │   └── JwtFilter.java
│   │   │   └── exceptions
│   │   │       ├── CustomException.java
│   │   │       └── GlobalExceptionHandler.java
│   │   └── resources
│   │       ├── static
│   │       ├── templates
│   │       └── application.properties
│
├── test
│   ├── java
│   │   ├── controllers
│   │   │   ├── AuthControllerTest.java
│   │   │   └── BankControllerTest.java
│   │   └── services
│   │       ├── AuthServiceTest.java
│   │       └── BankServiceTest.java
│
└── pom.xml
```lua
````
