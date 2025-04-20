# 🤔 O que são **Operadores Lógicos?**

Operadores lógicos são palavras (ou símbolos) que o computador usa para **tomar decisões mais inteligentes**.

Eles permitem **combinar condições**, ou seja, fazer **perguntas mais completas** como:

- Está sol **E** estou de folga?
- Estou com fome **OU** com vontade de comer?
- **NÃO** está chovendo?

Todas essas perguntas são respondidas com:
- ✅ **Verdadeiro** (true)
- ❌ **Falso** (false)

---

## 🧠 Para que servem?

Eles ajudam a montar **regras mais inteligentes**, como:

> “Se eu tiver dinheiro **E** o mercado estiver aberto, vou fazer compras.”

---

## 🔐 Os 3 principais operadores:

| Operador | Nome           | Significado                          |
|----------|----------------|--------------------------------------|
| `&&`     | **E (AND)**    | Só é verdadeiro se **tudo for verdadeiro** |
| ![simboloou](../assets/simboloOU.png)     | **OU (OR)**    | É verdadeiro se **pelo menos um** for verdadeiro |
| `!`      | **NÃO (NOT)**  | **Inverte** o valor (true vira false e vice-versa) |

---

## 🟩 1. **Operador E (`&&`)**

### 🧾 Regra:
> Só é verdadeiro se **as duas condições forem verdadeiras**.

### 💬 Exemplo:
> “Se eu tiver **dinheiro** **E** o **cinema estiver aberto**, eu vou.”

| Tem dinheiro? | Cinema aberto? | Vai?     |
|---------------|----------------|----------|
| ✅ Sim         | ✅ Sim          | ✅ Sim    |
| ✅ Sim         | ❌ Não          | ❌ Não    |
| ❌ Não         | ✅ Sim          | ❌ Não    |
| ❌ Não         | ❌ Não          | ❌ Não    |

### 🧑‍💻 Pseudocódigo:
```plaintext
tem_dinheiro <- verdadeiro
cinema_aberto <- verdadeiro

Se (tem_dinheiro && cinema_aberto) então
    Escreva("Pode ir ao cinema 🎬")
Senão
    Escreva("Não pode ir 😢")
FimSe
```

---

## 🟨 2. **Operador OU (`||`)**

### 🧾 Regra:
> É verdadeiro se **pelo menos uma condição for verdadeira**.

### 💬 Exemplo:
> “Se eu estiver com **fome** **OU** com **vontade**, eu como.”

| Com fome? | Com vontade? | Vai comer? |
|-----------|---------------|------------|
| ✅ Sim     | ❌ Não         | ✅ Sim     |
| ❌ Não     | ✅ Sim         | ✅ Sim     |
| ✅ Sim     | ✅ Sim         | ✅ Sim     |
| ❌ Não     | ❌ Não         | ❌ Não     |

### 🧑‍💻 Pseudocódigo:
```plaintext
com_fome <- falso
com_vontade <- verdadeiro

Se (com_fome || com_vontade) então
    Escreva("Vai comer 🍽️")
Senão
    Escreva("Não vai comer 🚫")
FimSe
```

---

## 🟥 3. **Operador NÃO (`!`)**

### 🧾 Regra:
> Ele **inverte** a resposta:
> - Se for verdadeiro → vira falso
> - Se for falso → vira verdadeiro

### 💬 Exemplo:
> “Se **NÃO** estiver chovendo, eu vou sair.”

| Está chovendo? | !Está chovendo? | Vai sair? |
|----------------|------------------|------------|
| ✅ Sim         | ❌ Falso          | ❌ Não     |
| ❌ Não         | ✅ Verdadeiro     | ✅ Sim     |

### 🧑‍💻 Pseudocódigo:
```plaintext
chovendo <- falso

Se (!chovendo) então
    Escreva("Pode sair de casa 🏃")
Senão
    Escreva("Melhor ficar em casa ☔")
FimSe
```
---

## 👩‍🏫 Dica da Profê:

> **Operadores lógicos** são como **conectores de perguntas**:
>
> - “Se isso **e** aquilo...”
> - “Se isso **ou** aquilo...”
> - “Se **não** isso...”

---

## 🎒 Atividade prática para sala:

**Situação:**  
Um aluno quer jogar videogame. Ele só pode jogar se:

- **Fez a lição**
- **E a mãe deixou**

```plaintext
fez_licao <- verdadeiro
mae_deixou <- falso

Se (fez_licao && mae_deixou) então
    Escreva("Pode jogar 🎮")
Senão
    Escreva("Não pode jogar 😢")
FimSe
```


