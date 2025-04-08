### 🧠 **O que é uma variável?**

Uma **variável** é como uma **caixa com etiqueta** onde você **guarda um valor** que pode mudar com o tempo.

#### 📦 Imagine assim:
- Uma variável é **uma caixinha**.
- Essa caixinha tem um **nome** (etiqueta).
- Dentro dela, você guarda **algum valor** (como um número, uma palavra, etc.).

---

### 💬 Exemplo do dia a dia:

Vamos usar o exemplo de uma **garrafa de água**.

- A garrafa tem um **rótulo** com o nome da pessoa: `aluno1`
- Dentro da garrafa está o **conteúdo**: `água`

Na lógica de programação, seria assim:

```plaintext
aluno1 = "água"
```

Isso significa: o nome da variável é `aluno1` e ela guarda o valor `"água"`.

---

### 🔁 O que é atribuição?

**Atribuição** é o ato de **colocar um valor dentro da variável**.  
Na programação, usamos o sinal **`=`** para isso.

#### 📌 Pense assim:
> A variável é a caixa → a atribuição é quando você **coloca algo dentro da caixa**.

---

### ✏️ Outro exemplo do cotidiano:

Imagine que você está anotando sua idade num papel:

```plaintext
idade = 20
```

Depois de um ano, você atualiza:

```plaintext
idade = 21
```

Isso quer dizer que a **variável `idade` agora vale 21**, substituindo o valor anterior.

---

### 🎒 Exemplo prático de uma mochila:

Você tem uma mochila que pode guardar um item por vez:

```plaintext
mochila = "livro"
```

Mais tarde, você troca:

```plaintext
mochila = "caderno"
```

Agora a mochila não tem mais o livro, ela tem um caderno.  
Isso mostra que **o valor da variável pode mudar**, mas o **nome dela continua o mesmo**.

---

### 🧾 Resumo simples:

| Conceito       | Explicação fácil                              | Exemplo                     |
|----------------|-----------------------------------------------|-----------------------------|
| Variável       | Uma caixinha com nome para guardar valores    | `nome = "João"`             |
| Atribuição     | Ação de guardar um valor na variável          | `nota = 9.5`                |
| Reatribuição   | Trocar o valor anterior por outro             | `nota = 7.0`                |

## Tipos de Variáveis

### 🏷️ **O que são tipos de variáveis?**
Os **tipos de variáveis** são como **categorias** que ajudam a entender que tipo de informação você está guardando.

### 🏷️ **Cada tipo de variável:**

- **Inteiro**: `idade = 20`
- **Flutuante**: `altura = 1.75`
- **String**: `nome = "Maria"`
- **Booleano**: `estudando = verdadeiro`
- **Lista**: `notas = [10, 8, 9]`
- **Dicionário**: `aluno = {"nome": "João", "idade": 20}`

### 🏷️ **Por que isso é importante?**

Os tipos de variáveis ajudam o computador a entender como **trabalhar com os dados**.
Por exemplo, se você tentar somar um número com uma palavra, o computador não vai entender.
#### **Exemplo de erro:**
```plaintext
soma = 10 + "5"  # Isso vai dar erro, porque não dá para somar um número com uma palavra.
```

### 📌 **Como escolher o tipo certo?**

- **Inteiro**: Use quando precisar de números inteiros (sem casas decimais).
- **Flutuante**: Use quando precisar de números com casas decimais.
- **String**: Use para texto (palavras, frases).
- **Booleano**: Use para verdadeiro ou falso (sim ou não).
- **Lista**: Use para guardar várias informações em uma única variável.
- **Dicionário**: Use para guardar informações em pares de chave-valor (como um mini banco de dados).

### 🏷️ **Quando utilizar cada tipo de variável**
- **Inteiro**: Para contagens, idades, quantidades.
Exemplo: `idade = 20`, `quantidade = 5`.

- **Flutuante**: Para medidas, notas, valores monetários.
Exemplo: `altura = 1.75`, `preco = 19.99`.

- **String**: Para nomes, endereços, textos.
Exemplo: `nome = "Maria"`, `endereco = "Rua A, 123"`.

- **Booleano**: Para condições, sim/não, verdadeiro/falso.
Exemplo: `estudando = verdadeiro`, `aprovado = falso`.

- **Lista**: Para coleções de itens, como notas, produtos.
Exemplo: `notas = [10, 8, 9]`, `produtos = ["maçã", "banana", "laranja"]`.

- **Dicionário**: Para informações estruturadas, como dados de um aluno (nome, idade, notas).
Exemplo: `aluno = {"nome": "João", "idade": 20, "notas": [10, 8, 9]}`.

🤯 Dica da Profê: **Use dicionários quando precisar de informações organizadas em pares de chave-valor, como um mini banco de dados.Não confunda com listas, que são apenas coleções de itens.**

### 🧾 **Resumo dos tipos de variáveis:**
| Tipo        | Exemplo                  | Descrição                          | Quando utilizar |
|-------------|--------------------------|------------------------------------|------------------|
| Inteiro     | `idade = 20`            | Números inteiros                   | Para contagens, idades, quantidades de números exatos|
| Flutuante  | `altura = 1.75`         | Números com casas decimais         | Para medidas, notas, valores monetários de números flutuantes|
| String      | `nome = "Maria"`        | Texto (palavras)                   |Para nomes, endereços, textos|
| Booleano    | `estudando = verdadeiro` | Verdadeiro ou falso                 |Para condições, sim/não, verdadeiro/falso |
| Lista       | `notas = [10, 8, 9]`    | Coleção de valores                 |Para listas de itens, como notas, produtos|
| Dicionário  | `aluno = {"nome": "João", "idade": 20}` | Estrutura de chave-valor          |Para informações organizadas, como dados de um aluno|