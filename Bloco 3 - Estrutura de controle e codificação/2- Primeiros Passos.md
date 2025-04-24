## 🧮 1. **Entrada e Saída**
### Objetivo: Pedir o nome do aluno e dar boas-vindas

```portugol
programa {
    funcao inicio() {
        cadeia nome

        escreva("Digite seu nome: ")
        leia(nome)

        escrevaLinha("Olá, ", nome, "! Seja bem-vindo(a)!")
    }
}
```

🧠 **Explicação:**  
Começamos com o mais básico: **pegar um valor e exibir uma mensagem**.  
Usamos `leia` e `escrevaLinha`, os primeiros comandos que todo iniciante precisa entender.

---

## ⚖️ 2. **Condicional `se`, `senao se`, `senao`**
### Objetivo: Dizer se o número é positivo, negativo ou zero

```portugol
programa {
    funcao inicio() {
        inteiro numero

        escreva("Digite um número: ")
        leia(numero)

        se (numero > 0) {
            escrevaLinha("O número é positivo.")
        } senao se (numero < 0) {
            escrevaLinha("O número é negativo.")
        } senao {
            escrevaLinha("O número é zero.")
        }
    }
}
```

🧠 **Explicação:**  
Introduzimos **decisões lógicas**, comparando valores para tomar caminhos diferentes no programa.

---

## 🔁 3. **Repetição com `para`**
### Objetivo: Contar de 1 até 5

```portugol
programa {
    funcao inicio() {
        para (inteiro i = 1; i <= 5; i++) {
            escrevaLinha("Número: ", i)
        }
    }
}
```

🧠 **Explicação:**  
Usamos o `para` para repetir um bloco de código com **controle numérico definido**.

---

## 🔁 4. **Repetição com `enquanto`**
### Objetivo: Contar até o número digitado

```portugol
programa {
    funcao inicio() {
        inteiro numero, i = 1

        escreva("Digite até onde contar: ")
        leia(numero)

        enquanto (i <= numero) {
            escrevaLinha(i)
            i = i + 1
        }
    }
}
```

🧠 **Explicação:**  
Mostramos como usar `enquanto`, útil para repetições **com condição baseada no valor digitado**.

---

## 🔁 5. **Repetição com `faca ... enquanto`**
### Objetivo: Repetir até o aluno digitar "ok"

```portugol
programa {
    funcao inicio() {
        cadeia resposta

        faca {
            escreva("Digite 'ok' para continuar: ")
            leia(resposta)
        } enquanto (resposta <> "ok")

        escrevaLinha("Você digitou 'ok'. Continuando...")
    }
}
```

🧠 **Explicação:**  
O `faca ... enquanto` garante que o bloco **seja executado pelo menos uma vez** antes de verificar a condição.

---

## 🧮 6. **Operadores de Comparação**
### Verificar igualdade, diferença e faixa de valores

```portugol
programa {
    funcao inicio() {
        inteiro idade

        escreva("Digite sua idade: ")
        leia(idade)

        se (idade == 18) {
            escrevaLinha("Você tem 18 anos.")
        } senao se (idade <> 18) {
            escrevaLinha("Você tem uma idade diferente de 18.")
        }

        se (idade >= 18 && idade <= 60) {
            escrevaLinha("Você está na faixa adulta.")
        }
    }
}
```

🧠 **Explicação:**  
Aqui combinamos operadores de comparação `==`, `<>`, `>=`, `<=` para validar **igualdade e faixas de valor**.

---

## 🔗 7. **Operadores Lógicos**
### Verificar múltiplas condições com `&&`, `||` e `nao`

```portugol
programa {
    funcao inicio() {
        logico temConvite
        inteiro idade

        escreva("Digite sua idade: ")
        leia(idade)

        escreva("Você tem convite? (verdadeiro/falso): ")
        leia(temConvite)

        se (idade < 5 || idade > 60) {
            escrevaLinha("Você tem direito à prioridade.")
        }

        se (nao temConvite) {
            escrevaLinha("Você não pode entrar.")
        }

        se (idade >= 18 && temConvite) {
            escrevaLinha("Entrada liberada!")
        }
    }
}
```

🧠 **Explicação:**  
Mostramos **como combinar condições** com os operadores `E`, `OU` e `NÃO`.

---

## 🛠️ 8. **Função**
### Objetivo: Somar dois números usando uma função

```portugol
programa {
    funcao inteiro somar(inteiro a, inteiro b) {
        retorne a + b
    }

    funcao inicio() {
        inteiro x, y, resultado

        escreva("Digite o primeiro número: ")
        leia(x)

        escreva("Digite o segundo número: ")
        leia(y)

        resultado = somar(x, y)

        escrevaLinha("A soma é: ", resultado)
    }
}
```

🧠 **Explicação:**  
Introduzimos **funções com retorno**, para **organizar o código** e facilitar reuso de cálculos.

---

## 🛠️ 9. **Procedimento**
### Objetivo: Mostrar uma mensagem de boas-vindas com procedimento

```portugol
programa {
    procedimento mostrarMensagem() {
        escrevaLinha("Bem-vindo(a) ao programa!")
    }

    funcao inicio() {
        mostrarMensagem()
    }
}
```

🧠 **Explicação:**  
Um **procedimento** é parecido com função, mas **não retorna valor**, apenas executa uma ação.

---

## 📦 10. **Matriz**
### Objetivo: Guardar e mostrar notas de 2 alunos com 3 provas

```portugol
programa {
    funcao inicio() {
        inteiro notas[2][3]
        inteiro i, j

        // Preencher notas
        para (i = 0; i < 2; i++) {
            para (j = 0; j < 3; j++) {
                escreva("Digite a nota ", j+1, " do aluno ", i+1, ": ")
                leia(notas[i][j])
            }
        }

        // Mostrar notas
        para (i = 0; i < 2; i++) {
            escreva("Notas do aluno ", i+1, ": ")
            para (j = 0; j < 3; j++) {
                escreva(notas[i][j], " ")
            }
            escrevaLinha()
        }
    }
}
```

🧠 **Explicação:**  
Trabalhamos agora com **matrizes**, ideais para **tabelas de dados**, como notas escolares.

