# 🧩 **Operadores Relacionais**
> São usados para **comparar valores** e dizer se uma **condição é verdadeira ou falsa**.

---

## 👶 Como explicar para iniciantes?

> Os operadores relacionais são como **perguntas de comparação**:
>
> - A idade é maior que 18?  
> - A nota é igual a 10?  
> - O preço é diferente de 0?

Essas perguntas sempre têm **resposta de SIM ou NÃO**, ou melhor:
- ✅ **Verdadeiro (true)**
- ❌ **Falso (false)**

---

## 📚 Quais são os operadores relacionais?

| Símbolo | Nome                       | Pergunta que faz                | Exemplo                 |
|---------|----------------------------|----------------------------------|-------------------------|
| `==`    | Igual a                    | "É igual?"                      | `5 == 5` → ✅ verdadeiro |
| `!=`    | Diferente de               | "É diferente?"                  | `3 != 5` → ✅ verdadeiro |
| `>`     | Maior que                  | "É maior?"                      | `10 > 7` → ✅ verdadeiro |
| `<`     | Menor que                  | "É menor?"                      | `4 < 2` → ❌ falso       |
| `>=`    | Maior ou igual a           | "É maior ou igual?"             | `7 >= 7` → ✅ verdadeiro |
| `<=`    | Menor ou igual a           | "É menor ou igual?"             | `5 <= 4` → ❌ falso      |

---

## 📦 Exemplos com linguagem do dia a dia:

### ✅ 1. `==` → Igual a  
> “A senha digitada é **igual** à senha correta?”

```plaintext
senha_digitada <- "1234"

Se (senha_digitada == "1234") então
    Escreva("Acesso liberado 🔓")
Senão
    Escreva("Senha incorreta ❌")
FimSe
```

---

### ❌ 2. `!=` → Diferente de  
> “A resposta está **diferente** do gabarito?”

```plaintext
resposta <- "B"

Se (resposta != "C") então
    Escreva("Resposta errada ❌")
Senão
    Escreva("Resposta certa ✅")
FimSe
```

---

### 🟩 3. `>` → Maior que  
> “A idade é **maior** que 18?”

```plaintext
idade <- 20

Se (idade > 18) então
    Escreva("É maior de idade ✅")
Senão
    Escreva("Ainda é menor de idade ❌")
FimSe
```

---

### 🟨 4. `<` → Menor que  
> “A temperatura está **menor** que 10 graus?”

```plaintext
temperatura <- 7

Se (temperatura < 10) então
    Escreva("Está frio! 🧥")
Senão
    Escreva("Temperatura agradável ☀️")
FimSe
```

---

### 🟦 5. `>=` → Maior ou igual a  
> “A média é **maior ou igual** a 7?”

```plaintext
media <- 7.5

Se (media >= 7) então
    Escreva("Aluno aprovado ✅")
Senão
    Escreva("Aluno reprovado ❌")
FimSe
```

---

### 🟥 6. `<=` → Menor ou igual a  
> “A velocidade está **menor ou igual** ao limite?”

```plaintext
velocidade <- 60
limite <- 60

Se (velocidade <= limite) então
    Escreva("Dentro do limite ✅")
Senão
    Escreva("Multado 🚨")
FimSe
```

---

## 👩‍🏫 Dica da Profê:

> **Operadores relacionais servem para comparar coisas.**
>
> Eles respondem perguntas do tipo:
> - Isso é igual?
> - Isso é maior?
> - Isso é menor?
> - Isso é diferente?

O resultado será sempre **verdadeiro** ou **falso**.

---

## 🎒 Atividade prática para sala:

**Crie um programa que:**
1. Peça a idade do usuário  
2. Compare com 16  
3. Diga se ele **pode votar**

**Pseudocódigo sugerido:**
```plaintext
Escreva("Digite sua idade:")
Leia(idade)

Se (idade >= 16) então
    Escreva("Pode votar 🗳️")
Senão
    Escreva("Ainda não pode votar ❌")
FimSe
```

