# Jornada do usuário

O **sistema** inicia com a criação do usuário.
O **usuário** acessa o sistema e realiza a autenticação.
Após autenticado com sucesso, o **usuário** ganha acesso ao aplicativo.
O **sistema** cria **uma conta** para aquele usuário na agência com saldo inicial.
O **usuário** visualiza o saldo da sua conta bancária atual.
Ao visualizar o saldo, o **usuário** tem as seguintes opções:
Registrar um depósito para aumentar o saldo da conta.
Realizar uma **transferência** de fundos para outra conta bancária.
Sacar dinheiro para retirar fundos da conta.
Ao escolher registrar um depósito:
O **usuário** insere o valor do depósito.
O sistema atualiza o saldo da conta após o depósito.
Ao escolher realizar uma transferência:
O **usuário** fornece os detalhes da conta de destino e o valor da transferência.
O **sistema** verifica a disponibilidade de saldo na conta.
Se houver saldo suficiente, o valor é transferido para a conta de destino.
Ao escolher sacar dinheiro:
O **usuário** insere o valor que deseja sacar.
O **sistema** verifica a disponibilidade de saldo na conta.
Se houver saldo suficiente, o **valor** é deduzido da conta e entregue ao usuário.
Após cada ação (depósito, transferência ou saque), o **usuário** pode visualizar novamente o saldo atualizado e o histórico de transações.

Cada sujeito (quem realiza a ação) foi separado do verbo (ação realizada)
Normalmente, o sujeito geralmente se torna uma entidade ou objeto, e o verbo representa as operações ou métodos que essa entidade pode executar.
Resumo:
O sistema inicia com a autenticação do usuário. Se o usuário foi autenticado, o usuário registra uma conta bancária. De posse de uma agência e uma conta, o usuário visualiza o seu saldo. Neste momento o usuário poderá registar um depósito, realizar uma transferência, sacar dinheiro.

1. Autenticação do Usuário:
   O sistema começa com a etapa de autenticação do usuário. Nesse ponto, o usuário precisa fornecer suas credenciais de login, geralmente compreendendo um nome de usuário e uma senha, ou outros métodos de autenticação seguros, como autenticação biométrica (impressão digital, reconhecimento facial, etc.). O sistema verifica as informações fornecidas pelo usuário para confirmar sua identidade.
2. Registro de Conta Bancária:
   Uma vez que o usuário é autenticado com sucesso, ele tem a opção de registrar uma conta bancária no sistema. Isso envolve a inserção de detalhes relevantes, como o número da agência e o número da conta, que são associados à conta bancária do usuário. Esses detalhes servirão como identificadores para suas transações.
3. Visualização do Saldo:
   Após o registro da conta bancária, o usuário pode acessar uma página ou seção onde visualizará o saldo atual da conta associada à agência e ao número da conta que ele registrou. Essa informação é obtida diretamente dos registros bancários e é apresentada de forma clara ao usuário.
4. Realização de Depósito:
   Com o saldo visível, o usuário tem a opção de registrar um depósito. Isso envolve inserir o valor que deseja depositar em sua conta bancária. O sistema valida a transação, atualiza o saldo com o valor depositado e registra essa transação no histórico do usuário.
5. Realização de Transferência:
   O usuário também tem a capacidade de realizar transferências de dinheiro entre suas próprias contas ou para contas de terceiros. Para isso, ele deve inserir os detalhes da conta de destino e o valor da transferência. O sistema verifica se os dados são válidos, atualiza os saldos das contas envolvidas e registra a transação.
6. Saque de Dinheiro:
   Além de depósitos e transferências, o sistema também permite que o usuário solicite um saque de dinheiro. O usuário insere o valor que deseja sacar e, se o saldo for suficiente, o sistema realiza a transação, deduzindo o valor sacado do saldo da conta.
