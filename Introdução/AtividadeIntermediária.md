## 🧠 Desafio 1 – **O Cofrinho de Juriscleyde**

### 📝 História:
Juriscleyde quer muito comprar um jogo novo que custa **100 moedas**. Para isso, ele guarda um valor diferente a cada dia no seu cofre. Seu desafio é criar um programa que acompanhe o progresso do Juriscleyde.

O programa deve começar com o total guardado em **zero**, e **repetir o processo de perguntar quanto Juriscleyde  guardou no dia**. Cada valor deve ser **somado ao total guardado**. Isso deve continuar **enquanto o total for menor que 100**.

Assim que o valor acumulado **atingir ou ultrapassar 100 moedas**, o programa deve parar e **mostrar uma mensagem de que o objetivo foi alcançado**.

### 🧩 Variáveis sugeridas:
- `valorDoDia`
- `totalGuardado`

---

## 🧠 Desafio 2 – **O Detector de Alienígenas**

### 📝 História:
Na Estação Espacial Internacional (ISS) e na Estação Espacial Tiangong (TSS) da China, todos os seres de outros planetas passam por um escaneamento ao chegar. O sistema precisa **verificar duas informações** de cada criatura:
- A **temperatura corporal**
- A **quantidade de olhos**

Uma criatura será marcada como **suspeita** se **tiver temperatura acima de 39** **OU** **se não tiver exatamente 2 olhos**.

Ou seja, o programa deve analisar as duas condições:
- Se **temperatura > 39**
- **OU** se **quantidade de olhos ≠ 2**

Se **qualquer uma dessas condições for verdadeira**, o programa deve **exibir uma mensagem dizendo que a criatura é suspeita**. Caso contrário, deve informar que ela é inofensiva.

### 🧩 Variáveis sugeridas:
- `temperatura`
- `quantidadeOlhos`
- `resultadoVerificacao`

---

## 🧠 Desafio 3 – **O Torneio dos Números**

### 📝 História:
Em um reino distante, existe um torneio onde dois números mágicos se enfrentam para descobrir quem é o mais poderoso. Seu programa deve **receber dois números** escolhidos pelos jogadores.

Ele deve então:
- Verificar se o **primeiro número é maior que o segundo**
- Se **for igual**, declarar **empate**
- Caso contrário, declarar que o **segundo número venceu**

Ou seja, o programa precisa analisar:
- Se **numeroUm > numeroDois**, declarar vencedor o primeiro
- **Senão se numeroDois > numeroUm**, o segundo vence
- **Senão**, houve empate

### 🧩 Variáveis sugeridas:
- `numeroUm`
- `numeroDois`
- `vencedor`

---

## 🧠 Desafio 4 – **A Senha Secreta da Caverna**

### 📝 História:
No Parque Municipal Morro Do Finder existe uma caverna misteriosa que guarda um grande tesouro. Mas só é possível entrar digitando a senha mágica correta: **"dragao123"**. O explorador tem até **3 tentativas** para acertar.

Seu programa deve começar com o número de tentativas em **zero** e pedir a senha. Se a senha **estiver correta**, uma mensagem de "Acesso liberado" deve ser mostrada.

Se a senha estiver **errada**, o número de tentativas deve **aumentar em 1**. O programa deve continuar **enquanto a senha estiver errada** **E** **o número de tentativas for menor que 3**.

Se as 3 tentativas forem usadas sem sucesso, o programa deve exibir uma mensagem de **"Acesso bloqueado"**.

### 🧩 Variáveis sugeridas:
- `senhaDigitada`
- `tentativas`
- `senhaMisteriosa` (valor fixo: "dragao123")

---

## 🧠 Desafio 5 – **A Receita do Bolo Inteligente**

### 📝 História:
Professora Kamylla começou a vida fitness, porém ela criou um programa para calcular se suas receitas são saudáveis. Ela quer saber **quantas calorias há em uma fatia de bolo**.

Você deve pedir quantas calorias tem cada ingrediente: **farinha, açúcar, ovos e manteiga**. Depois, pergunte em **quantas fatias o bolo será dividido**.

O programa deve **somar todas as calorias** dos ingredientes, **dividir pelo número de fatias**, e verificar se a **caloria por fatia for maior que 300**.

Se a pessoa estiver de dieta (indicar com **sim ou não**), e a **caloria por fatia for maior que 300**, o programa deve **mostrar um alerta** dizendo que essa receita talvez não seja ideal para a dieta.

Ou seja:
- Verificar se **caloriasPorFatia > 300** **E** **emDieta é verdadeiro**

### 🧩 Variáveis sugeridas:
- `caloriasFarinha`, `caloriasAcucar`, `caloriasOvos`, `caloriasManteiga`
- `caloriasTotais`
- `quantidadeFatias`
- `caloriasPorFatia`
- `emDieta`
- `mensagemAlerta`

