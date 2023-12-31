
# Sistema Bancário em C#

Este é um simples sistema bancário desenvolvido em C# que permite realizar operações básicas como saque, depósito e gerenciamento de contas e titulares.

## Funcionalidades

### 1. Conta Bancária
- **`ContaBancaria`**: Representa uma conta bancária e possui as propriedades:
    - `NumeroConta`: Número único da conta.
    - `Saldo`: Saldo atual da conta.
    - `Titular`: Referência ao titular da conta.

### 2. Titular da Conta
- **`TitularConta`**: Representa o titular da conta e contém:
    - `Nome`: Nome do titular.
    - `CPF`: Número de CPF do titular.

### 3. Operações
- **`Deposito(valor)`**: Método que realiza o depósito na conta.
- **`Saque(valor)`**: Método que realiza o saque da conta, se houver saldo suficiente.

## Exemplo de Uso

```csharp
// Criando um titular da conta
TitularConta titular = new TitularConta("João Silva", "123.456.789-10");

// Criando uma conta bancária para o titular
ContaBancaria conta = new ContaBancaria(1001, titular);

// Realizando operações na conta
conta.Deposito(500.00);
conta.Saque(200.00);
```

## Como Utilizar

1. Clone o repositório ou baixe os arquivos.
2. Abra o projeto em seu ambiente de desenvolvimento (Visual Studio, Visual Studio Code, etc.).
3. Compile e execute o código para interagir com o sistema bancário.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests para melhorias no sistema.

---

Esse README básico descreve as funcionalidades principais do sistema bancário em C#. Lembre-se de que isso é um exemplo simples e que um sistema bancário real teria muito mais complexidade e recursos de segurança implementados.
