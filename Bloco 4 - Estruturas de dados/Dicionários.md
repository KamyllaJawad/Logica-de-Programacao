### O que são **Dicionários**? 🔑

**Dicionários** são uma estrutura de dados em Python que armazenam **pares de chave-valor**. Ou seja, em vez de armazenar apenas um valor, como em uma lista ou tupla, o dicionário armazena um **valor associado a uma chave única**.

* **Chave (key)**: A chave é usada para identificar um valor. Ela é única dentro do dicionário e serve para acessar o valor correspondente.
* **Valor (value)**: O valor é o dado que está armazenado no dicionário e pode ser de qualquer tipo (número, string, lista, outro dicionário, etc.).

### Características dos **Dicionários**:

* **Desordenado**: Antes do Python 3.7, os dicionários não mantinham a ordem dos elementos. A partir do Python 3.7, os dicionários **mantêm a ordem** de inserção.
* **Mutáveis**: Os dicionários são mutáveis, ou seja, você pode **adicionar, remover ou modificar** elementos após a criação.
* **Chaves únicas**: As chaves em um dicionário são **únicas** e não podem se repetir. Se você tentar adicionar uma chave que já existe, o valor da chave será **atualizado**.

### Como criar um **Dicionário**?

Em Python, os dicionários são criados utilizando **chaves** `{}` e os pares de chave-valor são separados por dois pontos `:`.

```python
dicionario = {"nome": "João", "idade": 25, "profissao": "Engenheiro"}
```

Aqui, o dicionário tem 3 chaves: `"nome"`, `"idade"`, e `"profissao"`. Cada chave está associada a um valor.

---

### 1. **Exemplo Básico: Criando um dicionário simples**

Vamos criar um dicionário com informações sobre uma pessoa.

```python
pessoa = {"nome": "Maria", "idade": 30, "cidade": "São Paulo"}

# Acessando um valor pelo nome da chave
print(pessoa["nome"])  # Vai imprimir "Maria"
print(pessoa["idade"])  # Vai imprimir 30
```

**Explicação**: O dicionário `pessoa` tem três chaves: `"nome"`, `"idade"`, e `"cidade"`, com valores correspondentes a essas chaves. Para acessar o valor de uma chave, usamos a sintaxe `dicionario["chave"]`.

---

### 2. **Exemplo com alteração de valores**

Agora vamos mostrar como podemos **modificar o valor** de uma chave existente.

```python
pessoa = {"nome": "Carlos", "idade": 22, "cidade": "Rio de Janeiro"}

# Alterando a idade da pessoa
pessoa["idade"] = 23

# Exibindo o novo valor
print(pessoa["idade"])  # Vai imprimir 23
```

**Explicação**: O valor da chave `"idade"` foi alterado de 22 para 23. Como dicionários são mutáveis, podemos atualizar os valores a qualquer momento.

---

### 3. **Exemplo com adição de novos pares chave-valor**

Agora, vamos adicionar um novo par **chave-valor** ao dicionário.

```python
pessoa = {"nome": "Ana", "idade": 28}

# Adicionando uma nova chave "profissao"
pessoa["profissao"] = "Designer"

print(pessoa)
```

**Resultado esperado**:

```python
{"nome": "Ana", "idade": 28, "profissao": "Designer"}
```

**Explicação**: O dicionário agora tem uma nova chave `"profissao"`, associada ao valor `"Designer"`. Quando adicionamos uma nova chave a um dicionário, o valor correspondente a essa chave é inserido automaticamente.

---

### 4. **Exemplo com remoção de elementos**

É possível **remover** itens de um dicionário utilizando o comando `del` ou o método `pop()`.

```python
pessoa = {"nome": "Luiza", "idade": 27, "cidade": "Fortaleza"}

# Removendo a chave "cidade"
del pessoa["cidade"]

# Exibindo o dicionário após a remoção
print(pessoa)
```

**Resultado esperado**:

```python
{"nome": "Luiza", "idade": 27}
```

**Explicação**: A chave `"cidade"` foi removida do dicionário. Quando removemos uma chave, ela e o valor associado a ela são excluídos do dicionário.

---

### 5. **Exemplo com laço `for` para iterar sobre chaves e valores**

Você pode usar um **laço `for`** para percorrer as **chaves** e os **valores** de um dicionário.

```python
pessoa = {"nome": "Lucas", "idade": 21, "cidade": "Salvador"}

# Iterando sobre o dicionário
for chave, valor in pessoa.items():
    print(f"A chave é: {chave} e o valor é: {valor}")
```

**Resultado esperado**:

```python
A chave é: nome e o valor é: Lucas
A chave é: idade e o valor é: 21
A chave é: cidade e o valor é: Salvador
```

**Explicação**: O método `.items()` retorna **pares chave-valor** do dicionário. Com isso, podemos percorrer cada par de dados e exibi-los de maneira legível.

---

### **Resumo**

* **Dicionários** em Python são coleções de **pares chave-valor**.
* Eles são **mutáveis**, ou seja, você pode **adicionar, modificar e remover** elementos a qualquer momento.
* Para acessar um valor, você usa a **chave** correspondente.
* **Chaves** são únicas e não podem ser repetidas dentro do mesmo dicionário.
* O dicionário é **desordenado**, mas a partir do Python 3.7, ele **mantém a ordem de inserção**.

### **Exemplo Completo**

```python
# Criando um dicionário de uma pessoa
pessoa = {
    "nome": "Carla",
    "idade": 35,
    "cidade": "Curitiba"
}

# Modificando a idade
pessoa["idade"] = 36

# Adicionando uma nova chave
pessoa["profissao"] = "Arquiteta"

# Removendo a chave cidade
del pessoa["cidade"]

# Iterando sobre o dicionário
for chave, valor in pessoa.items():
    print(f"{chave}: {valor}")
```

**Resultado esperado**:

```python
nome: Carla
idade: 36
profissao: Arquiteta
```
