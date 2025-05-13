### 1. **Checagem de Senha 🔐**

**História:** Um sistema de segurança precisa liberar acesso apenas para quem digitar a senha correta.

**Atividade:**

* Solicite ao usuário uma senha.
* Compare com a senha correta: `"python123"`.
* Se for igual, exiba: `"Acesso liberado!"`.
* Se for diferente, exiba: `"Senha incorreta. Tente novamente."`

🧩 Interpretação: o usuário deve pensar na lógica de comparação exata entre textos.

---

### 2. **Verificador de Entrada de Cinema 🎬**

**História:** Você está na bilheteria de um cinema e precisa verificar se a pessoa pode pagar meia-entrada.

**Regras:**

* Menores de 18 anos ou maiores de 60 pagam meia.
* Os demais pagam inteira.

**Atividade:**

* Peça a idade do usuário.
* Diga se ele tem direito à meia-entrada ou não.

🧩 Interpretação: o aluno precisa compreender **dois critérios alternativos** usando `or`.

---

### 3. **Nome no Cartão de Acesso 🪪**

**História:** Uma empresa imprime cartões de acesso com nomes abreviados.

**Regras:**

* Se o nome tiver mais de 10 letras, mostrar: `"Nome muito longo para o cartão!"`.
* Caso contrário, mostrar: `"Nome válido para o cartão."`

**Atividade:**

* Peça o nome do usuário.
* Use `len()` para verificar o comprimento.

🧩 Interpretação: o aluno tem que contar os caracteres e aplicar lógica de comparação.

---

### 4. **Soma Somente dos Pares 🔢**

**História:** Você está criando um somador que só considera números pares de uma lista.

**Atividade:**

* Crie uma lista com **5 números inteiros fixos** no código (ex: `[1, 4, 7, 8, 10]`).
* Some **somente os números pares**.
* Exiba o resultado.

🧩 Interpretação: aplicar `if` **dentro de um `for`**.

---

### 5. **Verificador de Senha Forte 🛡️**

**História:** Você está ajudando seu amigo a saber se a senha que ele criou é segura.

**Critério de segurança:**

* Ter **8 caracteres ou mais**.
* Conter **pelo menos um número**.

**Atividade:**

* Peça uma senha ao usuário.
* Verifique o tamanho.
* Use a função `.isdigit()` dentro de um `for` para ver se tem número.
* Exiba: `"Senha forte!"` ou `"Senha fraca."`

🧩 Interpretação: aplicar `for` para varrer caracteres de uma `string`.

---

### 6. **Contagem Regressiva para o Evento ⏳**

**História:** Um evento vai começar em X segundos e você quer fazer uma contagem regressiva até 1.

**Atividade:**

* Peça ao usuário para digitar um número (ex: 5).
* Exiba a contagem regressiva até 1.

📌 Use o `for` com `range(valor, 0, -1)`.

🧩 Interpretação: o aluno precisa entender como **usar o `range` de forma decrescente**.

---

### 7. **Relatório de Compras 💰**

**História:** Você foi ao mercado e anotou 3 valores de compras. Agora quer saber:

* Qual foi o maior gasto
* Qual foi o menor
* E qual foi o total

**Atividade:**

* Peça os **3 valores** ao usuário (ex: 12.5, 6.75, 20).
* Mostre o maior, o menor e a soma total.

🧩 Interpretação: aplicar `max()`, `min()` e `sum()` com uma lista criada a partir de `input`.

---

### 8. **Palavra Secreta: Letra por Letra 🎯**

**História:** Uma brincadeira revela a “palavra secreta” letra por letra, como se fosse uma adivinhação.

**Atividade:**

* Peça ao usuário uma palavra.
* Mostre cada letra da palavra **em linha separada**, **precedida pela posição** (começando do 1).

📌 Exemplo:

```
1 - P
2 - y
3 - t
...
```

🧩 Interpretação: usar `for` com `range` .
