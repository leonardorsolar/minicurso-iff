# Gerenciamento da Sprint 1

**cgatGpt:** transforme as histórias de usuários e cenários de teste em tarefas menores e liste-as em checklist no formato markdown [ ] para o arquivo .md:

# Checklist de Tarefas

## História de Usuário 1 - Registro de Usuário (US001.1)

-   [ ] Criar página de registro de usuário com campos obrigatórios (nome, e-mail, senha).
-   [ ] Validar que todos os campos obrigatórios estão preenchidos.
-   [ ] Validar formato do e-mail (caso inválido, exibir mensagem de erro).
-   [ ] Implementar backend para registro de usuário e persistência no banco de dados.
-   [ ] Exibir mensagem de confirmação de registro bem-sucedido.

### Cenário de Sucesso

-   [ ] Testar registro de usuário com todos os campos preenchidos corretamente.
-   [ ] Confirmar criação da conta e exibição da mensagem de sucesso.

### Cenário de Erro: Campos Obrigatórios Não Preenchidos

-   [ ] Testar envio de formulário com campos obrigatórios em branco.
-   [ ] Verificar se a mensagem de erro de campos obrigatórios aparece corretamente.

### Cenário de Erro: E-mail Inválido

-   [ ] Testar envio de formulário com e-mail em formato inválido.
-   [ ] Verificar se a mensagem de erro de e-mail inválido é exibida corretamente.

---

## História de Usuário 2 - Validação de E-mail Duplicado (US001.2)

-   [ ] Criar verificação no backend para identificar e-mails já cadastrados.
-   [ ] Exibir mensagem de erro caso o e-mail já esteja em uso.

### Cenário de Sucesso

-   [ ] Testar registro com e-mail que não está registrado.
-   [ ] Confirmar criação de conta para um e-mail novo.

### Cenário de Erro: E-mail Já Registrado

-   [ ] Testar registro com e-mail já cadastrado.
-   [ ] Verificar se a mensagem de erro de "e-mail já registrado" é exibida.

---

## História de Usuário 3 - Login de Usuário (US002.1)

-   [ ] Criar página de login com campos para e-mail e senha.
-   [ ] Implementar backend para validação de credenciais e geração de token JWT.
-   [ ] Redirecionar o usuário para a página principal após login bem-sucedido.

### Cenário de Sucesso

-   [ ] Testar login com credenciais corretas.
-   [ ] Confirmar autenticação bem-sucedida e redirecionamento para a página principal.

### Cenário de Erro: E-mail ou Senha Incorretos

-   [ ] Testar login com e-mail incorreto.
-   [ ] Testar login com senha incorreta.
-   [ ] Verificar se a mensagem de erro de "e-mail ou senha incorretos" é exibida corretamente.

---

## História de Usuário 4 - Geração de Token JWT após Login (US002.2)

-   [ ] Implementar geração de token JWT no backend após autenticação bem-sucedida.
-   [ ] Armazenar o token JWT no lado do cliente para acessar rotas protegidas.
-   [ ] Configurar middleware para verificar o token JWT nas rotas protegidas.

### Cenário de Sucesso

-   [ ] Testar geração do token JWT após login bem-sucedido.
-   [ ] Confirmar que o token JWT é armazenado corretamente e pode ser usado em rotas protegidas.

### Cenário de Erro: Falha na Geração do Token JWT

-   [ ] Simular erro na geração do token JWT.
-   [ ] Verificar se o sistema exibe uma mensagem de erro adequada e impede o acesso a rotas protegidas.
