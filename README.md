# Sistema Bancário em Python / Banking System in Python

[English version below](#banking-system-in-python)

## Sistema Bancário em Python

Um sistema simples de gerenciamento bancário desenvolvido em Python, implementando conceitos de programação orientada a objetos, como herança, encapsulamento, composição e classes abstratas.

### Descrição

Este projeto simula as funcionalidades básicas de um sistema bancário, permitindo:
- Cadastro de clientes (pessoa física)
- Criação de contas correntes
- Operações financeiras (depósito e saque)
- Consulta de extrato
- Listagem de contas

O sistema foi desenvolvido utilizando boas práticas de programação, como:
- Programação orientada a objetos
- Aplicação de decoradores para logging
- Uso de tipos anotados (type hints)
- Métodos abstratos
- Encapsulamento de dados

### Estrutura do Projeto

#### Classes Principais

- `Cliente`: Classe base para representar um cliente do banco
- `PessoaFisica`: Classe derivada de Cliente para representar pessoas físicas
- `Conta`: Classe base para representar uma conta bancária
- `ContaCorrente`: Implementação específica de uma conta corrente com limites de saque
- `Transacao`: Classe abstrata para representar uma transação financeira genérica
- `Saque` e `Deposito`: Classes derivadas de Transação para implementar operações específicas
- `Historico`: Classe responsável por manter o histórico de transações

#### Funcionalidades

- Criação e gerenciamento de clientes
- Criação e gerenciamento de contas
- Realização de transações (saques e depósitos)
- Consulta de extrato (histórico de transações)
- Interface de linha de comando para interação com o usuário

### Como Executar

O programa pode ser executado diretamente via Python:

```bash
python desafio_poo.py
```

### Menu de Opções

Ao executar o programa, você terá acesso às seguintes opções:

1. **Depositar**: Realizar um depósito em uma conta
2. **Sacar**: Realizar um saque em uma conta
3. **Extrato**: Consultar o extrato de uma conta
4. **Nova conta**: Criar uma nova conta para um cliente existente
5. **Listar contas**: Listar todas as contas cadastradas
6. **Novo usuário**: Cadastrar um novo cliente
7. **Sair**: Encerrar o programa

### Limitações

- Cada cliente pessoa física possui apenas uma conta corrente
- A conta corrente possui limite de saque (R$ 500,00) e número máximo de saques (3)
- Dados são armazenados apenas em memória (não persistentes)

### Regras de Negócio

- Um cliente pode ter múltiplas contas
- Uma conta pertence a apenas um cliente
- Saques e depósitos devem ser de valores positivos
- Saques não podem exceder o saldo disponível
- Saques em conta corrente estão limitados a um valor máximo e quantidade de operações

### Tecnologias Utilizadas

- Python 3
- Biblioteca padrão Python:
  - abc (Abstract Base Classes)
  - datetime
  - textwrap
  - typing

### Possíveis Melhorias

- Implementação de persistência de dados
- Adição de outros tipos de conta (poupança, investimento)
- Implementação de transferências entre contas
- Suporte a diferentes tipos de cliente (pessoa jurídica)
- Interface gráfica para o usuário
- Melhoria no sistema de autenticação

### Autor

Marcus Lafaiete

---

## Banking System in Python

A simple banking management system developed in Python, implementing object-oriented programming concepts such as inheritance, encapsulation, composition, and abstract classes.

### Description

This project simulates the basic functionalities of a banking system, allowing:
- Customer registration (individuals)
- Current account creation
- Financial operations (deposit and withdrawal)
- Statement inquiry
- Account listing

The system was developed using good programming practices, such as:
- Object-oriented programming
- Application of decorators for logging
- Use of type hints
- Abstract methods
- Data encapsulation

### Project Structure

#### Main Classes

- `Cliente`: Base class to represent a bank customer
- `PessoaFisica`: Derived class from Cliente to represent individuals
- `Conta`: Base class to represent a bank account
- `ContaCorrente`: Specific implementation of a current account with withdrawal limits
- `Transacao`: Abstract class to represent a generic financial transaction
- `Saque` and `Deposito`: Classes derived from Transacao to implement specific operations
- `Historico`: Class responsible for maintaining the transaction history

#### Features

- Creation and management of customers
- Creation and management of accounts
- Performing transactions (withdrawals and deposits)
- Statement inquiry (transaction history)
- Command-line interface for user interaction

### How to Run

The program can be executed directly via Python:

```bash
python desafio_poo.py
```

### Menu Options

When running the program, you will have access to the following options:

1. **Deposit**: Make a deposit to an account
2. **Withdraw**: Make a withdrawal from an account
3. **Statement**: Check the statement of an account
4. **New account**: Create a new account for an existing customer
5. **List accounts**: List all registered accounts
6. **New user**: Register a new customer
7. **Exit**: Close the program

### Limitations

- Each individual customer has only one current account
- The current account has a withdrawal limit (R$ 500.00) and a maximum number of withdrawals (3)
- Data is stored only in memory (non-persistent)

### Business Rules

- A customer can have multiple accounts
- An account belongs to only one customer
- Withdrawals and deposits must be positive values
- Withdrawals cannot exceed the available balance
- Withdrawals from current accounts are limited to a maximum value and number of operations

### Technologies Used

- Python 3
- Python standard library:
  - abc (Abstract Base Classes)
  - datetime
  - textwrap
  - typing

### Possible Improvements

- Implementation of data persistence
- Addition of other account types (savings, investment)
- Implementation of transfers between accounts
- Support for different types of customers (legal entities)
- Graphical user interface
- Improvement in the authentication system

### Author

Marcus Lafaiete
