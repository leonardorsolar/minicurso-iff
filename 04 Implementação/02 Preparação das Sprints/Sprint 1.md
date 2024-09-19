## Sprint 1

    Duração: 2 semanas (01/10/2024 - 15/10/2024)
    Objetivos:
        Implementar funcionalidades básicas de login e registro.
        Configurar autenticação de dois fatores (2FA).
    Backlog:
        US001.1: Implementar login com e-mail e senha.
        US001.2: Implementar autenticação de dois fatores (2FA).
        US001.3: Implementar registro de usuário com e-mail e senha.

**cgatGpt:** transforme as funcionalidades a seguir em histórias de usuários e cenários de teste de aceitação do tipo Give, when, then:

# Histórias de Usuário e Cenários de Teste

## US001.1: Implementar login com e-mail e senha

História de Usuário: Como usuário, desejo realizar o login com e-mail e senha para acessar minha conta, para que eu possa acessar minhas informações pessoais e funcionalidades da conta de forma segura e conveniente.

Cenários de Teste de Aceitação:

    Cenário: Login bem-sucedido
        Dado que o usuário está na página de login,
        Quando ele insere um e-mail e senha válidos e clica no botão de login,
        Então ele deve ser redirecionado para a página principal da conta e ver uma mensagem de boas-vindas.

    Cenário: Login com credenciais incorretas
        Dado que o usuário está na página de login,
        Quando ele insere um e-mail ou senha incorretos e clica no botão de login,
        Então ele deve ver uma mensagem de erro informando que as credenciais estão incorretas.

    Cenário: Campos obrigatórios em branco
        Dado que o usuário está na página de login,
        Quando ele tenta fazer login sem preencher o e-mail ou a senha,
        Então ele deve ver uma mensagem de erro informando que os campos e-mail e senha são obrigatórios.

## US001.2: Implementar autenticação de dois fatores (2FA)

História de Usuário: Como usuário, desejo configurar a autenticação de dois fatores (2FA) para aumentar a segurança da minha conta, para que eu possa proteger melhor minha conta contra acessos não autorizados.

Cenários de Teste de Aceitação:

    Cenário: Configuração de 2FA bem-sucedida
        Dado que o usuário está na página de configurações de segurança,
        Quando ele ativa a autenticação de dois fatores e completa o processo de configuração com um código enviado para o e-mail ou aplicativo autenticador,
        Então ele deve ver uma confirmação de que a autenticação de dois fatores foi configurada com sucesso.

    Cenário: Login com 2FA ativado
        Dado que o usuário tem a autenticação de dois fatores ativada,
        Quando ele faz login com e-mail e senha válidos,
        Então ele deve ser solicitado a inserir um código de verificação enviado para seu e-mail ou aplicativo autenticador antes de acessar a conta.

    Cenário: Falha na autenticação de 2FA
        Dado que o usuário está na etapa de verificação de 2FA,
        Quando ele insere um código de verificação incorreto,
        Então ele deve ver uma mensagem de erro informando que o código de verificação está incorreto e deve tentar novamente.

## US001.3: Implementar registro de usuário com e-mail e senha

História de Usuário: Como novo usuário, desejo me registrar criando uma conta com e-mail e senha, para que eu possa acessar os serviços bancários e gerenciar minha conta.

Cenários de Teste de Aceitação:

    Cenário: Registro bem-sucedido
        Dado que o usuário está na página de registro,
        Quando ele preenche os campos de e-mail e senha e clica no botão de registrar,
        Então ele deve receber uma confirmação de que a conta foi criada com sucesso e deve receber um e-mail de verificação para confirmar seu e-mail.

    Cenário: Registro com e-mail já em uso
        Dado que o usuário está na página de registro,
        Quando ele preenche o campo de e-mail com um e-mail que já está registrado e tenta se registrar,
        Então ele deve ver uma mensagem de erro informando que o e-mail já está em uso e deve tentar um e-mail diferente.

    Cenário: Campos obrigatórios em branco no registro
        Dado que o usuário está na página de registro,
        Quando ele tenta se registrar sem preencher o e-mail ou a senha,
        Então ele deve ver uma mensagem de erro informando que os campos e-mail e senha são obrigatórios.

# Gerenciamento da Sprint 1

**cgatGpt:** transforme as histórias de usuários e cenários de teste em tarefas menores e liste-as em checklist no formato markdown [ ] :

## Checklist de Tarefas

## US001.1: Implementar login com e-mail e senha

**História de Usuário:**
Como usuário, desejo realizar o login com e-mail e senha para acessar minha conta, para que eu possa acessar minhas informações pessoais e funcionalidades da conta de forma segura e conveniente.

**Checklist:**

-   [ ] Criar a página de login com campos para e-mail e senha.
-   [ ] Implementar a validação de entrada para e-mail e senha não vazios.
-   [ ] Implementar a lógica de autenticação para verificar e-mail e senha.
-   [ ] Desenvolver a funcionalidade para redirecionar o usuário para a página principal após um login bem-sucedido.
-   [ ] Exibir uma mensagem de boas-vindas na página principal após o login.
-   [ ] Implementar a mensagem de erro para credenciais incorretas.
-   [ ] Criar testes automatizados para os seguintes cenários:
    -   [ ] **Cenário: Login bem-sucedido**
        -   [ ] Dado que o usuário está na página de login,
        -   [ ] Quando ele insere um e-mail e senha válidos e clica no botão de login,
        -   [ ] Então ele deve ser redirecionado para a página principal da conta e ver uma mensagem de boas-vindas.
    -   [ ] **Cenário: Login com credenciais incorretas**
        -   [ ] Dado que o usuário está na página de login,
        -   [ ] Quando ele insere um e-mail ou senha incorretos e clica no botão de login,
        -   [ ] Então ele deve ver uma mensagem de erro informando que as credenciais estão incorretas.
    -   [ ] **Cenário: Campos obrigatórios em branco**
        -   [ ] Dado que o usuário está na página de login,
        -   [ ] Quando ele tenta fazer login sem preencher o e-mail ou a senha,
        -   [ ] Então ele deve ver uma mensagem de erro informando que os campos e-mail e senha são obrigatórios.

---

## US001.2: Implementar autenticação de dois fatores (2FA)

**História de Usuário:**
Como usuário, desejo configurar a autenticação de dois fatores (2FA) para aumentar a segurança da minha conta, para que eu possa proteger melhor minha conta contra acessos não autorizados.

**Checklist:**

-   [ ] Criar a página de configurações de segurança.
-   [ ] Implementar a funcionalidade para ativar a autenticação de dois fatores.
-   [ ] Implementar o envio de código de verificação para o e-mail ou aplicativo autenticador.
-   [ ] Desenvolver a funcionalidade para o usuário inserir o código de verificação recebido.
-   [ ] Implementar a confirmação da configuração bem-sucedida de 2FA.
-   [ ] Adicionar uma etapa de verificação de 2FA durante o login quando a autenticação estiver ativada.
-   [ ] Criar testes automatizados para os seguintes cenários:
    -   [ ] **Cenário: Configuração de 2FA bem-sucedida**
        -   [ ] Dado que o usuário está na página de configurações de segurança,
        -   [ ] Quando ele ativa a autenticação de dois fatores e completa o processo de configuração com um código enviado para o e-mail ou aplicativo autenticador,
        -   [ ] Então ele deve ver uma confirmação de que a autenticação de dois fatores foi configurada com sucesso.
    -   [ ] **Cenário: Login com 2FA ativado**
        -   [ ] Dado que o usuário tem a autenticação de dois fatores ativada,
        -   [ ] Quando ele faz login com e-mail e senha válidos,
        -   [ ] Então ele deve ser solicitado a inserir um código de verificação enviado para seu e-mail ou aplicativo autenticador antes de acessar a conta.
    -   [ ] **Cenário: Falha na autenticação de 2FA**
        -   [ ] Dado que o usuário está na etapa de verificação de 2FA,
        -   [ ] Quando ele insere um código de verificação incorreto,
        -   [ ] Então ele deve ver uma mensagem de erro informando que o código de verificação está incorreto e deve tentar novamente.

---

## US001.3: Implementar registro de usuário com e-mail e senha

**História de Usuário:**
Como novo usuário, desejo me registrar criando uma conta com e-mail e senha, para que eu possa acessar os serviços bancários e gerenciar minha conta.

**Checklist:**

-   [ ] Criar a página de registro com campos para e-mail e senha.
-   [ ] Implementar a validação de entrada para e-mail e senha não vazios.
-   [ ] Implementar a lógica de registro para verificar se o e-mail já está em uso.
-   [ ] Desenvolver a funcionalidade para enviar um e-mail de verificação após o registro.
-   [ ] Implementar a confirmação de registro bem-sucedido e a verificação de e-mail.
-   [ ] Criar testes automatizados para os seguintes cenários:
    -   [ ] **Cenário: Registro bem-sucedido**
        -   [ ] Dado que o usuário está na página de registro,
        -   [ ] Quando ele preenche os campos de e-mail e senha e clica no botão de registrar,
        -   [ ] Então ele deve receber uma confirmação de que a conta foi criada com sucesso e deve receber um e-mail de verificação para confirmar seu e-mail.
    -   [ ] **Cenário: Registro com e-mail já em uso**
        -   [ ] Dado que o usuário está na página de registro,
        -   [ ] Quando ele preenche o campo de e-mail com um e-mail que já está registrado e tenta se registrar,
        -   [ ] Então ele deve ver uma mensagem de erro informando que o e-mail já está em uso e deve tentar um e-mail diferente.
    -   [ ] **Cenário: Campos obrigatórios em branco no registro**
        -   [ ] Dado que o usuário está na página de registro,
        -   [ ] Quando ele tenta se registrar sem preencher o e-mail ou a senha,
        -   [ ] Então ele deve ver uma mensagem de erro informando que os campos e-mail e senha são obrigatórios.
