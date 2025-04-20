# 🧭 **Estruturas de Decisão**
> Ou: Como ensinar o computador a **tomar decisões**, como a gente faz no dia a dia!

---

## 🧠 O que é uma Estrutura de Decisão?

Uma **estrutura de decisão** permite ao programa **escolher entre dois (ou mais) caminhos** com base em uma **condição verdadeira ou falsa**.

> 🧒 Pense assim:  
> “**Se** estiver chovendo, **então** levo guarda-chuva.  
> **Senão**, vou sem ele.”

---

## 💡 Por que usar isso?

Porque **nem sempre queremos que o programa faça a mesma coisa o tempo todo.**  
Às vezes, queremos que ele **reaja** dependendo da situação!

---

## ✅ Palavras-chave (em pseudocódigo):

- `Se` → Quando a condição for **verdadeira**
- `Senão` → Quando a condição for **falsa**
- `Senão Se` → Para verificar **outra condição**

---

## 🛠️ Estrutura básica em pseudocódigo:

```plaintext
Se (condição) então
   // faça algo
Senão
   // faça outra coisa
FimSe
```

---

## 🧃 Exemplo do dia a dia:

### 🎯 Situação:
> “Se eu tiver sede, então bebo água. Senão, continuo assistindo TV.”

```plaintext
tem_sede <- verdadeiro

Se (tem_sede) então
    Escreva("Beber água 💧")
Senão
    Escreva("Continuar vendo TV 📺")
FimSe
```

---

## 🎓 Exemplo com nota de aluno:

> “Se a média for maior ou igual a 7, o aluno está aprovado.  
Senão, reprovado.”

```plaintext
media <- 6.5

Se (media >= 7) então
    Escreva("Aluno aprovado ✅")
Senão
    Escreva("Aluno reprovado ❌")
FimSe
```

---

## 🔁 Usando `Senão Se` (mais de uma condição)

> “Se a idade for menor que 12, é criança.  
Senão se for menor que 18, é adolescente.  
Senão, é adulto.”

```plaintext
idade <- 15

Se (idade < 12) então
    Escreva("É uma criança 🧒")
Senão Se (idade < 18) então
    Escreva("É um adolescente 👦")
Senão
    Escreva("É um adulto 👨")
FimSe
```

---

## 👩‍🏫 Dica da Profê:

- 💡 **Toda decisão precisa de uma pergunta com resposta SIM ou NÃO**
- 📥 **A resposta SIM leva para um caminho, e o NÃO leva para outro**
- 🧩 **Use operadores lógicos (`e`, `ou`, `não`) para fazer perguntas mais completas**

---

## 🎯 Atividade prática para sala de aula:

### Situação:
Você quer montar um programa que decide o que fazer com base no clima:

> - Se estiver **chovendo** e **com frio**, exibe: “Levar casaco e guarda-chuva!”
> - Se só estiver **chovendo**, exibe: “Levar guarda-chuva!”
> - Se **não estiver chovendo**, exibe: “Pode sair tranquilo!”

**Desafio: Monte esse pseudocódigo com seus colegas!**