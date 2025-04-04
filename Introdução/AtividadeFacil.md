## 📘 Desafio 1 – Somar até chegar a 100

**Objetivo:** O aluno deve digitar números até que a soma total atinja ou ultrapasse 100.

### 🧠 Conceitos:
- Repetição `Enquanto`
- Operador matemático `+`

### 🔄 Lógica:
```plaintext
soma <- 0

Enquanto (soma < 100) faça
    Leia(numero)
    soma <- soma + numero
FimEnquanto

Escreva("Você atingiu ou passou de 100! ✅")
```

---

## 📘 Desafio 2 – Verificar se número é par ou ímpar

**Objetivo:** O usuário digita um número e o programa informa se é **par** ou **ímpar**.

### 🧠 Conceitos:
- Condição `Se...Senão`
- Operador matemático `%` (módulo)

### 🔄 Lógica:
```plaintext
Leia(numero)

Se (numero % 2 == 0) então
    Escreva("É par ⚖️")
Senão
    Escreva("É ímpar 🔢")
FimSe
```

---

## 📘 Desafio 3 – Perguntar idade até encontrar um adulto

**Objetivo:** O programa repete a pergunta da idade até que alguém tenha 18 anos ou mais.

### 🧠 Conceitos:
- Repetição `Enquanto`
- Condição `>=`

### 🔄 Lógica:
```plaintext
idade <- 0

Enquanto (idade < 18) faça
    Leia(idade)
FimEnquanto

Escreva("Maior de idade encontrado! 🎉")
```

---

## 📘 Desafio 4 – Verificar se pode entrar na festa

**Objetivo:** A pessoa só pode entrar na festa se tiver **mais de 18 anos** **e** **nome na lista**.

### 🧠 Conceitos:
- Condição com operador lógico `E`
- Comparação `>` e igualdade `==`

### 🔄 Lógica:
```plaintext
Leia(idade)
Leia(nome)

Se (idade > 18 && nome == "João") então
    Escreva("Pode entrar na festa 🎉")
Senão
    Escreva("Entrada negada 🚫")
FimSe
```

💡 Dica: pode testar com vários nomes e idades diferentes!

---

## 📘 Desafio 5 – Login com limite de tentativas

**Objetivo:** O usuário tem **3 tentativas** para digitar a senha correta.

### 🧠 Conceitos:
- Repetição `Enquanto`
- Condição composta com operador lógico `E`
- Contador e comparação

### 🔄 Lógica:
```plaintext
tentativas <- 0
senha <- ""

Enquanto (senha != "1234" && tentativas < 3) faça
    Leia(senha)
    tentativas <- tentativas + 1
FimEnquanto

Se (senha == "1234") então
    Escreva("Acesso permitido 🔓")
Senão
    Escreva("Acesso bloqueado 🚫")
FimSe
```

