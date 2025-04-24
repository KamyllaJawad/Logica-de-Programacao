
### 🧠 Desafio 1 – **O Cofrinho do Troco**
**História:**  
Ana tem o costume de guardar o troco que sobra das compras. Ela quer saber **quantas vezes** vai precisar guardar dinheiro até juntar pelo menos **200 moedas**.

📌 O seu programa começa com **total igual a zero**.  
📌 Depois, ele deve **repetir** o processo de pedir quanto foi guardado.  
📌 Cada valor deve ser **somado ao total guardado**.  
📌 A repetição deve continuar **ENQUANTO (WHILE)** o total for **menor que 200**.  
📌 Ao final, mostre **quantas vezes** Ana precisou guardar dinheiro.

🔧 Variáveis: `valor`, `total`, `vezes`  
🧠 Você vai precisar usar:
- Comando de **repetição ENQUANTO**
- Operador **< (menor que)**
- Operador **+ (soma)**

---

### 🧠 Desafio 2 – **O Verificador de Primos**
**História:**  
Um número é chamado de **primo** se ele só pode ser dividido por 1 e por ele mesmo (por exemplo: 2, 3, 5, 7, 11...).  
Você deve pedir **um número** ao usuário e **verificar se ele é primo ou não**.

📌 Para isso, conte **quantas vezes** esse número é divisível por algum número entre 1 e ele mesmo.  
📌 Use um **laço PARA** (FOR) para testar de 1 até o número.  
📌 Se ele for divisível **mais que 2 vezes**, então **NÃO é primo**.  
📌 Para verificar se um número é divisível, use o operador **% (módulo)**: se `numero % i == 0`, ele é divisível por `i`.

🔧 Variáveis: `numero`, `contador`, `i`  
🧠 Você vai precisar usar:
- Comando de **repetição PARA**
- Operador **% (módulo)**
- Condicional **SE...SENAO**
- Operador **== (igual a)**

---

### 🧠 Desafio 3 – **A Missão dos Três Números**
**História:**  
Três guerreiros trouxeram números mágicos para um desafio. Você precisa **descobrir qual é o maior número entre os três**.

📌 Peça três números diferentes.  
📌 Compare os três com **condições SE...SENÃO SE...SENÃO**.  
📌 Use o operador **> (maior que)** para descobrir qual deles é o maior.

🔧 Variáveis: `a`, `b`, `c`, `maior`  
🧠 Você vai precisar usar:
- Condicionais **SE**, **SENÃO SE** e **SENÃO**
- Operadores **> (maior que)**

---

### 🧠 Desafio 4 – **A Prova dos Pares**
**História:**  
Durante uma prova, o aluno digita **5 números**. Seu programa deve **contar quantos deles são pares**.

📌 Use um **laço PARA** (FOR) que repete 5 vezes.  
📌 A cada número digitado, use o operador **% (módulo)** para ver se o resto da divisão por 2 é zero.  
📌 Se for, **conte como par**.  
📌 No final, mostre quantos números pares foram digitados.

🔧 Variáveis: `numero`, `i`, `pares`  
🧠 Você vai precisar usar:
- Comando de **repetição PARA**
- Condicional **SE**
- Operador **% (módulo)** e **==**

---

### 🧠 Desafio 5 – **Caça à Palavra Secreta**
**História:**  
Seu programa vai pedir uma palavra. O usuário deve digitar a palavra secreta: **"liberdade"**.  
📌 Se digitar errado, o programa mostra “Tente novamente”.  
📌 Isso deve se repetir **ENQUANTO (WHILE)** a palavra estiver **diferente de "liberdade"**.

🔧 Variáveis: `palavra`  
🧠 Você vai precisar usar:
- Comando de **repetição ENQUANTO**
- Operador **≠ (diferente)** — no Portugol WebStudio: `<>`
- Comparação de texto (cadeia)

---

### 🧠 Desafio 6 – **O Elevador de Silvério**
**História:**  
Silvério só pode usar o elevador se estiver com um peso entre **50kg e 120kg**.

📌 Peça o peso do usuário.  
📌 Verifique com **duas comparações** usando os operadores **>= (maior ou igual a)** e **<= (menor ou igual a)**.  
📌 Use o operador **E (&&)** para garantir que as duas condições são verdadeiras.

🔧 Variáveis: `peso`  
🧠 Você vai precisar usar:
- Condicional **SE...SENÃO**
- Operadores **>=**, **<=**
- Operador lógico **E (&&)**

---

### 🧠 Desafio 7 – **A Calculadora de Média**
**História:**  
O aluno deve digitar **duas notas**. O programa calcula a **média** e diz se ele está aprovado.

📌 Se a média for **maior ou igual a 7**, ele **passou**.  
📌 Se for **menor que 7**, ele **reprovou**.  
📌 Use a fórmula: `(nota1 + nota2) / 2`.

🔧 Variáveis: `nota1`, `nota2`, `media`  
🧠 Você vai precisar usar:
- Operadores **+ (soma)** e **/ (divisão)**
- Condicional **SE...SENÃO**
- Operador **>= (maior ou igual a)**

---

### 🧠 Desafio 8 – **A Aposta dos Dados**
**História:**  
Dois amigos apostam e jogam um dado 3 vezes cada. Seu programa deve **somar os pontos** e dizer quem venceu.

📌 Repita o sorteio **3 vezes** para cada jogador.  
📌 Você pode **ler manualmente** os valores ou simular usando números.  
📌 No final, compare os totais usando **condicional SE...SENÃO SE...SENÃO** para decidir o vencedor ou se houve empate.

🔧 Variáveis: `pontos1`, `pontos2`, `i`, `dado`  
🧠 Você vai precisar usar:
- Comando de **repetição PARA**
- Condicional **SE...SENÃO**
- Operadores **+**, **>**, **==**

---

### 🧠 Desafio 9 – **O Múltiplo Misterioso**
**História:**  
Seu programa deve verificar se um número é **múltiplo de 3 e de 5 ao mesmo tempo**.

📌 Um número é múltiplo se o **resto da divisão por ele for zero** (use o **%**).  
📌 Use **SE** para verificar se ele **é divisível por 3 E por 5** (ou seja: `numero % 3 == 0 && numero % 5 == 0`).

🔧 Variáveis: `numero`  
🧠 Você vai precisar usar:
- Operador **% (módulo)**
- Operador lógico **E (&&)**
- Condicional **SE...SENÃO**

---

### 🧠 Desafio 10 – **A Fila do Sorvete**
**História:**  
Você trabalha numa sorveteria. Ao todo, **10 clientes** vão passar no seu caixa. Cada um vai dizer quantas bolas de sorvete quer.  
📌 O programa deve **somar o total de bolas vendidas no final**.

🔧 Variáveis: `bolas`, `total`, `i`  
🧠 Você vai precisar usar:
- Comando de **repetição PARA**
- Operador **+ (soma)**

