## 🧮 1. **Entrada e Saída**

### Objetivo: Receber dados e exibir uma mensagem formatada

```portugol
programa {
    funcao inicio() {
        cadeia nome
        inteiro idade

        limpa()

        escreva("Digite seu nome: ")
        leia(nome)

        escreva("Digite sua idade: ")
        leia(idade)

        escreva("Olá, ", nome, ". Você tem ", idade, " anos.")
    }
}
```

🧠 **Explicação:**  
Esse exemplo usa:
- `limpa()` para limpar a tela antes da interação;
- `leia()` para capturar entradas;
- `escreva()` e `escreva()` para saída de dados.

---

## 🧠 2. **Declaração de Tipos**

### Objetivo: Mostrar diferentes tipos de variáveis

```portugol
programa {
    funcao inicio() {
        inteiro idade = 25
        real altura = 1.75
        caracter inicial = 'A'
        cadeia nome = "Maria"
        logico aprovado = verdadeiro

        escreva("Nome: ", nome)
        escreva("Idade: ", idade)
        escreva("Altura: ", altura)
        escreva("Inicial: ", inicial)
        escreva("Aprovado: ", aprovado)
    }
}
```

🧠 **Explicação:**  
Apresenta os **tipos primitivos** da linguagem: `inteiro`, `real`, `caracter`, `cadeia`, `logico`.

---

## 📦 3. **Declaração de Estruturas**

### Objetivo: Usar diferentes tipos de declarações em Portugol

#### 1. Constantes
```portugol
// Exemplo 1: Constante para valor fixo
constante real PI = 3.14159
constante inteiro ANO_ATUAL = 2024

programa {
    funcao inicio() {
        real raio = 5
        real area = PI * raio * raio
        escreva("A área do círculo é: ", area, "\n")
        escreva("Estamos no ano de ", ANO_ATUAL)
    }
}

// Exemplo 2: Constante para texto
constante cadeia MENSAGEM = "Bem-vindo ao sistema!"
constante cadeia SENHA = "123456"

programa {
    funcao inicio() {
        escreva(MENSAGEM, "\n")
        escreva("A senha padrão é: ", SENHA)
    }
}

// Exemplo 3: Interativo - Usando constantes com entrada do usuário
constante real TAXA_JUROS = 0.05

programa {
    funcao inicio() {
        real valor_investido
        escreva("Digite o valor que deseja investir: ")
        leia(valor_investido)
        
        real rendimento = valor_investido * TAXA_JUROS
        escreva("Com a taxa de ", TAXA_JUROS * 100, "% você terá um rendimento de: ", rendimento)
    }
}
```

#### 2. Vetores
```portugol
// Exemplo 1: Vetor de números
programa {
    funcao inicio() {
        // Declaração e inicialização de um vetor de 5 números
        inteiro numeros[5] = {10, 20, 30, 40, 50}
        
        // Exibindo os valores do vetor
        para (inteiro i = 0; i < 5; i++) {
            escreva("Posição ", i, ": ", numeros[i], "\n")
        }
    }
}

// Exemplo 2: Vetor de nomes
programa {
    funcao inicio() {
        // Declaração e inicialização de um vetor de 3 nomes
        cadeia nomes[3] = {"João", "Maria", "Pedro"}
        
        // Alterando um valor do vetor
        nomes[1] = "Ana"
        
        // Exibindo os nomes
        para (inteiro i = 0; i < 3; i++) {
            escreva("Aluno ", i+1, ": ", nomes[i], "\n")
        }
    }
}

// Exemplo 3: Interativo - Preenchendo vetor com entrada do usuário
programa {
    funcao inicio() {
        // Declaração de um vetor vazio
        inteiro idades[5]
        
        // Preenchendo o vetor com idades digitadas pelo usuário
        para (inteiro i = 0; i < 5; i++) {
            escreva("Digite a idade da pessoa ", i+1, ": ")
            leia(idades[i])
        }
        
        // Exibindo as idades
        escreva("\nIdades digitadas:\n")
        para (inteiro i = 0; i < 5; i++) {
            escreva("Pessoa ", i+1, ": ", idades[i], " anos\n")
        }
    }
}
```

#### 3. Matrizes
```portugol
// Exemplo 1: Matriz de notas
programa {
    funcao inicio() {
        // Declaração de uma matriz 3x2 (3 alunos, 2 notas cada)
        real notas[3][2] = {{7.5, 8.0}, 
                           {6.0, 9.5}, 
                           {8.5, 7.0}}
        
        // Exibindo as notas
        para (inteiro aluno = 0; aluno < 3; aluno++) {
            escreva("Aluno ", aluno+1, ":\n")
            para (inteiro prova = 0; prova < 2; prova++) {
                escreva("  Prova ", prova+1, ": ", notas[aluno][prova], "\n")
            }
        }
    }
}

// Exemplo 2: Matriz de tabuleiro
programa {
    funcao inicio() {
        // Declaração de uma matriz 3x3 (tabuleiro)
        caracter tabuleiro[3][3] = {{'X', 'O', 'X'},
                                  {'O', 'X', 'O'},
                                  {'X', 'O', 'X'}}
        
        // Exibindo o tabuleiro
        para (inteiro linha = 0; linha < 3; linha++) {
            para (inteiro coluna = 0; coluna < 3; coluna++) {
                escreva(tabuleiro[linha][coluna], " ")
            }
            escreva("\n")
        }
    }
}

// Exemplo 3: Interativo - Preenchendo matriz com entrada do usuário
programa {
    funcao inicio() {
        // Declaração de uma matriz 2x2 vazia
        real numeros[2][2]
        
        // Preenchendo a matriz com números digitados pelo usuário
        para (inteiro linha = 0; linha < 2; linha++) {
            para (inteiro coluna = 0; coluna < 2; coluna++) {
                escreva("Digite o número para posição [", linha, "][", coluna, "]: ")
                leia(numeros[linha][coluna])
            }
        }
        
        // Exibindo a matriz
        escreva("\nMatriz digitada:\n")
        para (inteiro linha = 0; linha < 2; linha++) {
            para (inteiro coluna = 0; coluna < 2; coluna++) {
                escreva(numeros[linha][coluna], " ")
            }
            escreva("\n")
        }
    }
}
```

#### 4. Procedimentos
```portugol
// Exemplo 1: Procedimento simples
procedimento mostrarMensagem() {
    escreva("Olá! Este é um procedimento simples.\n")
}

// Exemplo 2: Procedimento com parâmetros
procedimento mostrarSoma(inteiro a, inteiro b) {
    inteiro resultado = a + b
    escreva("A soma de ", a, " + ", b, " = ", resultado, "\n")
}

// Exemplo 3: Interativo - Procedimento com entrada do usuário
procedimento calcularIMC() {
    real peso, altura, imc
    
    escreva("Digite seu peso (em kg): ")
    leia(peso)
    
    escreva("Digite sua altura (em metros): ")
    leia(altura)
    
    imc = peso / (altura * altura)
    escreva("Seu IMC é: ", imc, "\n")
    
    se (imc < 18.5) {
        escreva("Classificação: Abaixo do peso\n")
    } senao se (imc < 25) {
        escreva("Classificação: Peso normal\n")
    } senao se (imc < 30) {
        escreva("Classificação: Sobrepeso\n")
    } senao {
        escreva("Classificação: Obesidade\n")
    }
}

programa {
    funcao inicio() {
        mostrarMensagem()
        mostrarSoma(5, 3)
        mostrarSoma(10, 20)
        calcularIMC()
    }
}
```

#### 5. Funções
```portugol
// Exemplo 1: Função para calcular área do retângulo
funcao real calcularArea(real base, real altura) {
    retorne base * altura
}

// Exemplo 2: Função para verificar se um número é par
funcao logico ehPar(inteiro numero) {
    se (numero % 2 == 0) {
        retorne verdadeiro
    }
    retorne falso
}

// Exemplo 3: Interativo - Função com entrada do usuário
funcao real calcularMedia() {
    real nota1, nota2, nota3
    
    escreva("Digite a primeira nota: ")
    leia(nota1)
    
    escreva("Digite a segunda nota: ")
    leia(nota2)
    
    escreva("Digite a terceira nota: ")
    leia(nota3)
    
    retorne (nota1 + nota2 + nota3) / 3
}

programa {
    funcao inicio() {
        // Usando a função calcularArea
        real area = calcularArea(5.0, 3.0)
        escreva("Área do retângulo: ", area, "\n")
        
        // Usando a função ehPar
        inteiro num = 10
        se (ehPar(num)) {
            escreva(num, " é par\n")
        } senao {
            escreva(num, " é ímpar\n")
        }
        
        // Usando a função calcularMedia
        real media = calcularMedia()
        escreva("A média das notas é: ", media, "\n")
    }
}
```

🧠 **Explicação:**  
Cada tipo de declaração tem seu propósito específico:

1. **Constantes**: 
   - Valores que não mudam durante a execução do programa
   - Úteis para valores fixos como PI, configurações, etc.
   - Podem ser usadas em cálculos com entrada do usuário

2. **Vetores**: 
   - Armazenam uma lista de valores do mesmo tipo
   - Úteis para guardar sequências de dados relacionados
   - Podem ser preenchidos com dados digitados pelo usuário

3. **Matrizes**: 
   - Armazenam dados em formato tabular (linhas e colunas)
   - Úteis para representar dados bidimensionais
   - Podem ser preenchidas com dados digitados pelo usuário

4. **Procedimentos**: 
   - Executam ações sem retornar valores
   - Úteis para organizar código e evitar repetição
   - Podem solicitar e processar entrada do usuário

5. **Funções**: 
   - Executam ações e retornam valores
   - Úteis para cálculos e verificações
   - Podem solicitar dados do usuário e retornar resultados

**Observações importantes:**
- Vetores e matrizes começam no índice 0
- Procedimentos não retornam valores
- Funções sempre retornam um valor
- Constantes não podem ser alteradas após a declaração
- Use nomes descritivos para melhor entendimento do código
- Sempre valide as entradas do usuário para evitar erros

---

## ⚖️ 4. **Desvios Condicionais**

### Objetivo: Usar `se`, `senao se`, `senao` e `escolha caso`

```portugol
programa {
    funcao inicio() {
        inteiro opcao

        escreva("1 - Iniciar")
        escreva("2 - Ajuda")
        escreva("3 - Sair")
        escreva("Escolha uma opção: ")
        leia(opcao)

        escolha (opcao) {
            caso 1:
                escreva("Você escolheu iniciar.")
                pare
            caso 2:
                escreva("Você escolheu ajuda.")
                pare
            caso 3:
                escreva("Saindo do sistema.")
                pare
            padrao:
                escreva("Opção inválida.")
        }
    }
}
```

🧠 **Explicação:**  
Mostra como aplicar **decisões múltiplas** com `escolha` e `caso`, além dos tradicionais `se`, `senao se`, `senao`.

---

## 🔁 5. **Laços de Repetição**

### Objetivo: Usar os 3 tipos de laço (`para`, `enquanto`, `faca enquanto`)

```portugol
programa {
    funcao inicio() {
        inteiro i = 1

        escreva("Contando de 1 a 5 com PARA:")
        para (i = 1; i <= 5; i++) {
            escreva(i, " ")
        }

        escreva("\nContando de 1 a 5 com ENQUANTO:")
        i = 1
        enquanto (i <= 5) {
            escreva(i, " ")
            i = i + 1
        }

        escreva("\nUsando FACA ENQUANTO (para parar com 'ok'):")
        cadeia entrada
        faca {
            escreva("Digite 'ok' para parar: ")
            leia(entrada)
        } enquanto (entrada <> "ok")
    }
}
```

🧠 **Explicação:**  
Demonstra os três laços de repetição com finalidades diferentes:
- `para` com contador,
- `enquanto` com condição lógica,
- `faca enquanto` com execução obrigatória mínima.

---

## 🧠 6. **Operações Relacionais (Comparação)**

```portugol
programa {
    funcao inicio() {
        inteiro idade

        escreva("Digite sua idade: ")
        leia(idade)

        se (idade == 18) {
            escreva("Você tem 18 anos.")
        }

        se (idade <> 18) {
            escreva("Você não tem 18 anos.")
        }

        se (idade >= 60) {
            escreva("Idoso.")
        } senao se (idade <= 12) {
            escreva("Criança.")
        } senao {
            escreva("Adulto.")
        }
    }
}
```

🧠 **Explicação:**  
Aplicação prática dos comparadores: `==`, `<>`, `>=`, `<=`, `>`, `<`.

---

## 🔗 7. **Operações Lógicas**

```portugol
programa {
    funcao inicio() {
        inteiro idade
        logico temConvite

        escreva("Digite a idade: ")
        leia(idade)

        escreva("Tem convite? (verdadeiro ou falso): ")
        leia(temConvite)

        se (idade >= 18 e temConvite) {
            escreva("Entrada permitida.")
        } senao se (idade < 18 ou nao temConvite) {
            escrevaLinha("Entrada negada.")
        }
    }
}
```

🧠 **Explicação:**  
Mostra os operadores lógicos:
- `e` (E lógico),
- `ou` (OU lógico),
- `nao` (negação).

