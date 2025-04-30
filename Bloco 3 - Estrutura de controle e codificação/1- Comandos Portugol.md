## 🧮 **Entrada e Saída**

| **Comando** | **Descrição**                              | **Quando usar**                                     | **Como usar**                  | **Erros comuns**                                      |
|-------------|---------------------------------------------|------------------------------------------------------|--------------------------------|--------------------------------------------------------|
| `escreva`   | Exibe texto na tela (sem pular linha)       | Quando quiser exibir algo e continuar na mesma linha | `escreva("Nome: ")`            | Esquecer as aspas, vírgulas ou usar variável não declarada |
| `leia`      | Lê um valor digitado pelo usuário           | Para receber valores de entrada                     | `leia(nome)`                   | Usar variável não declarada antes                      |
| `limpa`     | Limpa a tela                                | Para limpar o terminal entre etapas do programa     | `limpa()`                      | Esquecer os parênteses ou não usar antes de novo menu  |

---

## 🧠 **Declaração de Tipos**

| **Tipo**     | **Descrição**                        | **Exemplo de uso**           | **Quando usar**                                 |
|--------------|---------------------------------------|-------------------------------|--------------------------------------------------|
| `inteiro`    | Número sem casas decimais             | `inteiro idade`               | Idades, contadores, opções numéricas             |
| `real`       | Número com casas decimais             | `real preco`                  | Preços, médias, cálculos com vírgula             |
| `caracter`   | Um único caractere                    | `caracter letra`              | Letras individuais (ex: 'A')                     |
| `cadeia`     | Um texto (string)                     | `cadeia nome`                 | Nomes, mensagens                                 |
| `logico`     | Verdadeiro ou falso                   | `logico aprovado`             | Situações booleanas                              |
| `vazio`      | Sem valor (usado em funções que não retornam) | `procedimento limparTela()` | Procedimentos que apenas executam ações         |

---

## 📦 **Declaração de Estruturas**

| **Comando**     | **Descrição**                                     | **Exemplo**                       |
|------------------|--------------------------------------------------|-----------------------------------|
| `variavel`       | Criação de variáveis                             | `inteiro idade`                   |
| `constante`      | Criação de um valor fixo                         | `constante inteiro LIMITE = 10`   |
| `vetor`          | Lista de dados em **uma dimensão**               | `cadeia nomes[10]`                |
| `matriz`         | Lista de dados em **duas dimensões**             | `real notas[3][2]`                |
| `funcao`         | Retorna um valor                                 | `funcao inteiro soma(...)`        |
| `procedimento`   | Não retorna valor (apenas executa ação)          | `procedimento mostrarMensagem()`  |

---

## ⚖️ **Desvios Condicionais**

| **Comando**      | **Descrição**                                        | **Quando usar**                                                | **Exemplo**                         |
|------------------|------------------------------------------------------|-----------------------------------------------------------------|-------------------------------------|
| `se`             | Executa algo **se** uma condição for verdadeira      | Verificar condições simples                                     | `se (idade > 18) { ... }`           |
| `senao se`        | Verifica nova condição, caso a anterior falhe       | Comparar **várias alternativas**                                | `senao se (idade == 18) { ... }`    |
| `senao`          | Executa algo se **todas as anteriores falharem**     | Oferecer um caminho "padrão"                                   | `senao { ... }`                     |
| `escolha caso`   | Escolhe o que executar entre **vários casos fixos**  | Quando a variável tem **valores exatos** para verificar         | `escolha(opcao) { caso 1: ... }`    |

---

## 🔁 **Laços de Repetição**

| **Comando**      | **Descrição**                                         | **Quando usar**                                            | **Exemplo**                                 |
|------------------|------------------------------------------------------|-------------------------------------------------------------|---------------------------------------------|
| `enquanto`       | Executa enquanto a condição for **verdadeira**       | Quando **não se sabe quantas vezes** irá repetir            | `enquanto (i < 10) { ... }`                 |
| `faca enquanto`  | Executa **pelo menos uma vez**, depois verifica      | Quando quer executar **uma vez antes de testar a condição** | `faca { ... } enquanto (condicao)`          |
| `para`           | Executa um bloco com **controle numérico**           | Quando já se sabe **quantas vezes** quer repetir            | `para (i = 1; i <= 5; i++) { ... }`         |

---

## 🧠 **Operações Relacionais (Comparações)**

| **Operador**  | **Significado**      | **Exemplo**              |
|---------------|----------------------|---------------------------|
| `==`          | Igual a              | `se (a == b)`             |
| `<>`          | Diferente de         | `se (a <> b)`             |
| `>`           | Maior que            | `se (idade > 18)`         |
| `<`           | Menor que            | `se (idade < 18)`         |
| `>=`          | Maior ou igual a     | `se (nota >= 7)`          |
| `<=`          | Menor ou igual a     | `se (idade <= 12)`        |

---

## 🔗 **Operações Lógicas**

| **Operador** | **Significado**                 | **Exemplo**                              |
|--------------|----------------------------------|-------------------------------------------|
| `e`         | E lógico (as duas são verdadeiras) | `se (idade > 18 && nome == "João")`       |
| `ou`         | OU lógico (uma ou outra é verdadeira) | `se (idade < 5 || idade > 60)`          |
| `nao`        | Nega a condição (inverso lógico) | `se (nao temConvite)`                    |
