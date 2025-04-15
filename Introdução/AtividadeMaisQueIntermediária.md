## 🧠 Desafio 1 – **O Elevador da Torre Misteriosa**

### 📝 História:
Na torre mágica de Altissia, o elevador só aceita andares entre **1 e 20**. Qualquer tentativa fora desse intervalo é ignorada.

Seu desafio é fazer um programa que:
- Peça ao usuário para informar o número do andar desejado.
- **Valide a entrada**: o número deve estar **entre 1 e 20**.
- Se o número for válido, exiba: `"Indo para o andar X..."`.
- Caso contrário, exiba: `"Andar inválido. Tente novamente."` e repita a pergunta **até um andar válido ser informado**.

### 🧩 Variáveis sugeridas:
- `andar`
- `andarValido` (booleano)

---

## 🧠 Desafio 2 – **A Triagem dos Aventureiros**

### 📝 História:
Antes de entrar na missão final, cada aventureiro deve passar por uma triagem. O sistema deve:
- Perguntar **a idade** e **o nível de energia** do aventureiro (de 0 a 100).
- Validar que a idade esteja entre **16 e 60 anos** e a energia entre **0 e 100**.
- Se **qualquer valor for inválido**, repetir a coleta até receber valores válidos.
- Depois, se o aventureiro tiver **mais de 30 anos** ou **energia acima de 70**, ele é considerado **Pronto para a missão**.
- Caso contrário, é **Recomendado descansar antes**.

### 🧩 Variáveis sugeridas:
- `idade`, `energia`
- `mensagemTriagem`

---
Claro! Vamos entender didaticamente **como funciona o desafio da Tabuada Inversa usando a estrutura `PARA` (FOR)** no Flowgorithm ou em qualquer linguagem com lógica semelhante.

---

## 🧠 Desafio 8 – **Tabuada Inversa da Sabedoria Ancestral**  
**Objetivo:** Exibir a tabuada de um número **de 10 até 1**, usando **exclusivamente o comando PARA** (FOR).

---

### 🧩 1. **Entrada do Usuário com Validação**

Antes de tudo, precisamos garantir que o número esteja no intervalo correto (**entre 1 e 10**).

**Lógica da validação:**
```plaintext
enquanto (numero < 1 OU numero > 10) faça
    peça o número novamente
```

➡️ Isso impede que a pessoa insira números negativos, zero, ou maiores que 10.

---

### 🧩 2. **O que é o comando PARA (FOR)?**

A estrutura `PARA` é usada quando **sabemos exatamente quantas vezes o laço será repetido**.

**Formato:**
```plaintext
PARA i de X até Y faça
   // comandos
FIMPARA
```

Mas e se quisermos contar **de trás para frente**?

👉 Podemos fazer assim:

```plaintext
PARA i de 10 até 1 passo -1 faça
```

Ou, no Flowgorithm:
```plaintext
for i = 10 to 1 step -1
```

---

### 🧩 3. **Lógica Interna do PARA**

Agora que temos a variável `numero` e sabemos que `i` irá de 10 até 1, a lógica é simples:

**Em cada repetição:**
- Multiplicamos `numero * i`
- Exibimos o resultado

---

### ✅ Exemplo Passo a Passo (com número 3):

| Valor de `i` | Operação     | Resultado |
|--------------|--------------|-----------|
| 10           | 3 x 10       | 30        |
| 9            | 3 x 9        | 27        |
| ...          | ...          | ...       |
| 1            | 3 x 1        | 3         |

---

### 📜 Código pseudolinguagem (estilo Flowgorithm)

```plaintext
declare numero, i, resultado como inteiro

escreva "Digite um número entre 1 e 10:"
leia numero

enquanto numero < 1 ou numero > 10 faça
    escreva "Valor inválido. Digite entre 1 e 10:"
    leia numero
fimenquanto

para i de 10 até 1 passo -1 faça
    resultado ← numero * i
    escreva numero + " x " + i + " = " + resultado
fimpara
```

---

### 🧠 Por que usar PARA?

- Porque sabemos exatamente **quantas vezes** queremos repetir (de 10 até 1 → são 10 repetições).
- O comando `PARA` **controla automaticamente** o valor de `i`, **sem precisar incrementar ou decrementar manualmente**.
- O uso de `passo -1` permite que o loop funcione em **ordem decrescente**.
