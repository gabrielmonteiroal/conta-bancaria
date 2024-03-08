# Conta Bancária Java

Este é um exercício de orientação a objetos feito em Java, é um exemplo simples de uma aplicação de conta bancária que utiliza o paradigma de orientação a objetos. Ele permite o cadastro de contas bancárias, com a opção de incluir um valor de depósito inicial. O saldo da conta pode ser atualizado por meio de depósitos e saques, e é aplicada uma taxa de $5.00 para cada saque.

## Funcionalidades
- Cadastro de uma nova conta bancária
- Opção de depósito inicial ao criar a conta
- Depósito de dinheiro na conta
- Saque de dinheiro da conta com aplicação de taxa

## Detalhes do Problema
Para cadastrar uma conta bancária, é necessário fornecer o número da conta, o nome do titular e, opcionalmente, um valor de depósito inicial. O número da conta é único e não pode ser alterado após a criação da conta. O nome do titular pode ser alterado, mas o número da conta permanecerá o mesmo.

O saldo da conta só pode ser alterado por meio de depósitos e saques. Cada saque tem uma taxa de $5.00, que é deduzida do saldo após o saque. Se o saldo não for suficiente para cobrir o valor do saque mais a taxa, a conta pode ficar com saldo negativo.

## Como Usar
1. Ao iniciar o programa, será solicitado o número da conta, o nome do titular e se há um depósito inicial.
2. Se for informado um depósito inicial, será solicitado o valor desse depósito.
3. Após o cadastro da conta, o programa exibirá os dados da conta.
4. Você poderá então realizar operações de depósito e saque.
5. Para cada saque, será deduzida uma taxa de $5.00 do saldo da conta.

## Estrutura do Código
- `Main.java`: Contém o método `main` onde o programa é iniciado. Aqui são feitas as interações com o usuário para criar e operar as contas bancárias.
- `Account.java`: A classe `Account` representa uma conta bancária. Ela possui métodos para depositar, sacar e mostrar informações da conta.

## Execução
Certifique-se de ter o Java JDK instalado em seu sistema.
1. Compile os arquivos `.java`:
   ```bash
   javac program/Main.java entities/Account.java
   ```
2. Execute o programa:
   ```bash
   java program.Main
   ```

## Exemplo de Uso
```
Enter account number: 12345
Enter account holder: John Doe
Is there an initial deposit (y/n)? y
Enter initial deposit value: 1000.00

Account data:
Account 12345, Holder: John Doe, Balance: $ 1000.00

Enter a deposit value: 500.00
Updated account data:
Account 12345, Holder: John Doe, Balance: $ 1500.00

Enter a withdraw value: 200.00
Updated account data:
Account 12345, Holder: John Doe, Balance: $ 1295.00
```

Este é um exemplo básico de como a aplicação pode ser utilizada. Experimente criar novas contas, realizar operações de depósito e saque para explorar as funcionalidades disponíveis.

---
