<p align="center">
  <img src="https://raw.githubusercontent.com/LucVinicius-DEV/exceptions2-java/main/banner.png" alt="Banner exceptions2-java" />
</p>

# exceptions2-java

Repositório criado durante o curso de Java do professor **Nélio Alves**.

Este projeto demonstra um **exemplo completo de tratamento de exceções em um sistema bancário**, abordando:

- Validações de regras de negócio (saldo, limite de saque, valores negativos)  
- Exceção personalizada `WithdrawException`  
- Estrutura limpa com pacotes de entidade e exceção  
- Mensagens de erro claras e responsabilidade bem separada  

---

### 📁 Estrutura do projeto

```
exceptions2-java/
├── src/
│   ├── application/
│   │   └── Program.java
│   └── model/
│       ├── entities/
│       │   └── Account.java
│       └── exceptions/
│           └── WithdrawException.java
```

---

### 💡 Conceitos aplicados

- **Exceção Personalizada (`WithdrawException`)** – lançada sempre que as regras de saque são violadas.  
- **Validações de Negócio** – saldo insuficiente, limite excedido, valores inválidos.  
- **Responsabilidade Separada** – validação na entidade, tratamento no `main`.  
- **Encapsulamento** – lógica crítica protegida dentro de `Account`.

---

### ✅ Exemplo de uso

```java
Account acc = new Account(number, holder, balance, withdrawLimit);

try {
    acc.withdraw(amount);
    System.out.println("New balance: " + acc.getBalance());
} catch (WithdrawException e) {
    System.out.println("Withdraw error: " + e.getMessage());
}
```

---

### 👨‍🏫 Professor

Projeto baseado nas aulas do [Prof. Nélio Alves](https://github.com/nelioalves), do curso **Java COMPLETO** na Udemy.

---

### 🔗 Licença

Este repositório é de uso educacional e foi criado para fins de estudo e prática em Java.
````0
