<p align="center">
  <img src="https://raw.githubusercontent.com/LucVinicius-DEV/exceptions2-java/main/banner.png" alt="Banner exceptions2-java" />
</p>

# Tratando exceções em Java

Repositório criado durante o curso de Java do professor **Nélio Alves**.

Este projeto demonstra um **exemplo completo de tratamento de exceções em contexto de aplicação real**, simulando um sistema bancário com:

- Validações e regras de negócio
- Exceções personalizadas
- Estrutura limpa com pacotes de entidade e exceção
- Boas práticas de encapsulamento e mensagens de erro claras

---

### 📁 Estrutura do projeto

```
exceptions2-java/
├── application/
│   └── Program.java
├── model/
│   └── entities/
│       └── Account.java
│   └── exceptions/
│       └── DomainException.java
```

---

### 💡 Conceitos aplicados

- **Exceções Personalizadas** – domínio controlando regras e lançando mensagens significativas.  
- **Validações de Regras de Negócio** – como saldo insuficiente, limites de saque, valores inválidos.  
- **Responsabilidade Separada** – tratamento no `main`, validação no modelo.  
- **Encapsulamento** – lógica crítica protegida na entidade `Account`.

---

### ✅ Exemplo de uso

```java
Account acc = new Account(number, holder, balance, withdrawLimit);
acc.withdraw(amount);
System.out.println("New balance: " + acc.getBalance());
```

---

### 👨‍🏫 Professor

Projeto baseado nas aulas do [Prof. Nélio Alves](https://github.com/nelioalves), do curso **Java COMPLETO** na Udemy.

---

### 🔗 Licença

Este repositório é de uso educacional e foi criado para fins de estudo e prática em Java.
