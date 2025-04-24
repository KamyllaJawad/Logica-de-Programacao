
# 🧮 **Comandos de Entrada e Saída**

| **Comando**    | **O que é**                             | **Quando usar**                                 | **Como usar**                                   | **Erros comuns**                              |
|----------------|------------------------------------------|--------------------------------------------------|--------------------------------------------------|------------------------------------------------|
| `escreva`      | Mostra texto na tela (sem pular linha)   | Quando quiser exibir mensagens ou variáveis      | `escreva("Olá ")`                                | Esquecer aspas ou vírgulas                      |
| `escrevaLinha` | Mostra texto e pula linha                | Ao exibir algo e querer pular para próxima linha | `escrevaLinha("Tudo bem?")`                     | Usar sem aspas ou com variável não declarada    |
| `leia`         | Lê valor do teclado                      | Quando quiser receber dados do usuário           | `leia(nome)`                                     | Ler sem declarar a variável antes              |

# 🔁 **Comandos de Repetição**

| **Comando**         | **O que é**                                           | **Quando usar**                                                                 | **Como usar**                                                                 | **Erros comuns**                                         |
|---------------------|------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------|----------------------------------------------------------|
| `para`              | Laço com contador                                    | Quando souber o número de repetições exatas                                     | `para (inteiro i = 1; i <= 10; i++) { ... }`                                   | Esquecer `i++` ou errar condição de parada               |
| `enquanto`          | Laço com condição                                    | Quando não souber o número de repetições, mas tiver uma condição                | `enquanto (x < 5) { ... }`                                                    | Esquecer de atualizar a variável e criar laço infinito   |
| `faca ... enquanto` | Laço que garante ao menos uma execução               | Quando precisa que o bloco rode pelo menos uma vez                              | `faca { ... } enquanto (condicao)`                                            | Não usar ponto e vírgula no final da condição (`;`)      |

# ⚖️ **Comandos Condicionais**

| **Comando** | **O que é**                                      | **Quando usar**                                              | **Como usar**                                                    | **Erros comuns**                                   |
|-------------|--------------------------------------------------|---------------------------------------------------------------|-------------------------------------------------------------------|----------------------------------------------------|
| `se`        | Condição (if)                                    | Quando quiser executar algo só se uma condição for verdadeira | `se (idade >= 18) { ... }`                                       | Esquecer os parênteses ou usar `=` ao invés de `==`|
| `senao se`  | Outra verificação caso a primeira falhe          | Quando tiver várias possibilidades de condição                | `senao se (idade > 12) { ... }`                                   | Repetir `se` em vez de `senao se`                 |
| `senao`     | Código para quando todas as condições falham     | Quando quiser uma alternativa caso nenhuma condição atenda    | `senao { ... }`                                                   | Colocar condição no `senao` (não pode ter)         |

# 📦 **Declaração de Variáveis**

| **Tipo**     | **O que é**                              | **Quando usar**                                    | **Como usar**                             | **Erros comuns**                                     |
|--------------|-------------------------------------------|-----------------------------------------------------|--------------------------------------------|------------------------------------------------------|
| `inteiro`    | Número sem casas decimais                 | Contagens, idades, índices                          | `inteiro idade`                            | Usar ponto em vez de vírgula (`10.5` em vez de `10`) |
| `real`       | Número com casas decimais                 | Alturas, preços, médias                             | `real preco`                                | Erros de arredondamento com comparação               |
| `cadeia`     | Texto                                     | Nomes, mensagens                                    | `cadeia nome`                               | Concatenar sem vírgula                               |
| `caracter`   | Um único caractere                        | Letras individuais                                  | `caracter letra`                            | Usar aspas duplas em vez de simples (`'a'` e não `"a"`) |
| `logico`     | Verdadeiro ou falso                       | Verificações (ex: login, aprovado)                 | `logico aprovado`                           | Comparar como se fosse número                        |


# 📊 **Declaração de Matrizes**

| **Comando** | **O que é**                                          | **Quando usar**                                                      | **Como usar**                                                | **Erros comuns**                                                  |
|-------------|------------------------------------------------------|-----------------------------------------------------------------------|---------------------------------------------------------------|-------------------------------------------------------------------|
| `matriz`    | Uma estrutura que armazena valores em **linhas e colunas** | Quando você precisa armazenar dados em formato de tabela (ex: jogo da velha, notas de alunos, mapas) | `inteiro matriz[3][3]` → cria uma matriz 3x3 de inteiros       | Esquecer de definir os tamanhos ou acessar fora dos limites (`matriz[3][3]` com índice inválido) |

# 🛠️ **Funções e Procedimentos**

| **Comando**         | **O que é**                                           | **Quando usar**                                                             | **Como usar**                                                                 | **Erros comuns**                                      |
|---------------------|------------------------------------------------------|------------------------------------------------------------------------------|--------------------------------------------------------------------------------|-------------------------------------------------------|
| `funcao`            | Bloco que **retorna** valor                         | Quando precisa de um resultado, como soma, média                             | `funcao inteiro soma(inteiro a, inteiro b) { retorne a + b }`                | Esquecer `retorne` ou retornar tipo errado            |
| `procedimento`      | Bloco que **não retorna** valor                     | Quando apenas quer executar algo (ex: mostrar mensagem)                      | `procedimento mostrar() { escreva("Oi") }`                                   | Tentar usar `retorne` ou atribuir retorno             |

# 🔎 **Operadores de Comparação**

| **Significado**        | **Símbolo em Portugol** | **Exemplo**                          | **Resultado esperado**                 |
|------------------------|--------------------------|---------------------------------------|----------------------------------------|
| Igual a                | `==`                     | `se (idade == 18)`                   | Verdadeiro se idade for exatamente 18 |
| Diferente de           | `<>`                     | `se (nome <> "João")`               | Verdadeiro se nome não for "João"     |
| Maior que              | `>`                      | `se (nota > 7)`                      | Verdadeiro se nota for maior que 7    |
| Menor que              | `<`                      | `se (nota < 7)`                      | Verdadeiro se nota for menor que 7    |
| Maior ou igual a       | `>=`                     | `se (idade >= 60)`                  | Verdadeiro se idade for 60 ou mais    |
| Menor ou igual a       | `<=`                     | `se (idade <= 12)`                  | Verdadeiro se idade for até 12        |


# 🧠 **Operadores Lógicos**

| **Significado**          | **Símbolo em Portugol** | **Exemplo**                                                  | **Resultado esperado**                                      |
|--------------------------|--------------------------|---------------------------------------------------------------|-------------------------------------------------------------|
| E (ambas as condições)   | `&&`                     | `se (idade > 18 && nome == "João")`                         | Verdadeiro só se as duas forem verdadeiras                 |
| OU (uma ou outra)        | `||`                     | `se (idade < 5 || idade > 60)`                              | Verdadeiro se pelo menos uma for verdadeira                |
| NÃO (negação)            | `nao`                    | `se (nao temConvite)`                                       | Verdadeiro se `temConvite` for falso                       |


