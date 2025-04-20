
## 🎓 **Mini Simulado – Lógica Limpa e Sem Gambiarra**  
**Tema:** *Criar código claro, correto e lógico – sem "viajar na maionese"!*

> 🧠 Cada questão tem uma alternativa correta. As demais ilustram **erros comuns**, inclusive "gambiarras criativas" que devem ser evitadas.

---

### ✅ **Questão 1: Variável correta**
Qual é a forma correta de declarar uma variável para guardar a idade de uma pessoa?

a) `20 = idade`  
b) `idade ← "vinte anos"`  
c) `idade ← 20`  
d) `var idade == 20`

✅ **Resposta correta:** **c)** `idade ← 20`

---

### ✅ **Questão 2: Evitando a gambiarra de texto**
Qual é o erro neste pseudocódigo?

```plaintext
nota ← "7"
Se (nota >= 6) então
    Escreva("Aprovado")
FimSe
```

a) Está perfeito  
b) Está comparando texto com número  
c) Está faltando o Senão  
d) A variável nota deveria se chamar notaFinal

✅ **Resposta correta:** **b)** Está comparando **texto com número**

---

### ✅ **Questão 3: Estrutura de repetição adequada**
Em um programa que precisa repetir **exatamente 10 vezes**, qual estrutura é mais adequada?

a) Enquanto  
b) Se  
c) Para  
d) Repita até

✅ **Resposta correta:** **c)** Para

---

### ✅ **Questão 4: Operador lógico correto**
Qual operador é usado para verificar se **duas condições** são verdadeiras ao mesmo tempo?

a) `||`  
b) `==`  
c) `&&`  
d) `!=`

✅ **Resposta correta:** **c)** `&&` (E lógico)

---

### ✅ **Questão 5: Lógica sem enrolação**
Qual é o erro da lógica abaixo?

```plaintext
Se (idade > 18) então
    Escreva("Maior de idade")
Senão Se (idade > 18) então
    Escreva("Talvez seja maior?")
FimSe
```

a) Está duplicando a mesma condição  
b) Está faltando variável  
c) Está faltando FimEnquanto  
d) Está certo sim!

✅ **Resposta correta:** **a)** Condição repetida sem necessidade (confunde o programa!)

---

### ✅ **Questão 6: Repetição correta para contagem regressiva**
Você quer exibir a tabuada do número 4 de 10 até 1. Qual estrutura você usaria?

a) `Para i de 1 até 10`  
b) `Para i de 10 até 1 passo -1`  
c) `Enquanto i < 10`  
d) `Repita até i == 0`

✅ **Resposta correta:** **b)** `Para i de 10 até 1 passo -1`

---

### ✅ **Questão 7: Evitando viagem**
Qual dessas instruções é **uma gambiarra perigosa**?

a) `media ← (nota1 + nota2) / 2`  
b) `Se (media >= 7) então Escreva("Aprovado")`  
c) `nota1 ← "cinco" + 3`  
d) `idade ← 20`

✅ **Resposta correta:** **c)** Está tentando somar texto com número – erro lógico!

---

### ✅ **Questão 8: Condição composta correta**
Qual condição representa corretamente: “Se o aluno tiver nota maior que 7 **e** frequência maior que 75”?

a) `nota > 7 || frequencia > 75`  
b) `nota == 7 && frequencia == 75`  
c) `nota > 7 && frequencia > 75`  
d) `nota != 7 || frequencia < 75`

✅ **Resposta correta:** **c)** `nota > 7 && frequencia > 75`

---

### ✅ **Questão 9: Reatribuição**
Após declarar `nome ← "João"`, como trocar o nome para "Lucas"?

a) `nome == "Lucas"`  
b) `nome ← "Lucas"`  
c) `Lucas ← nome`  
d) `nome = nome + "Lucas"`

✅ **Resposta correta:** **b)** `nome ← "Lucas"`

---

### ✅ **Questão 10: Cuidado com comparações erradas**
O que acontece com este código?

```plaintext
numero ← 5
Se (numero = 10) então
    Escreva("É dez")
Senão
    Escreva("Não é dez")
FimSe
```

a) Vai mostrar “É dez”  
b) Vai dar erro porque `=` não compara  
c) Está comparando certo  
d) Está esquecendo o FimPara

✅ **Resposta correta:** **b)** Está usando `=` em vez de `==` para comparar!
