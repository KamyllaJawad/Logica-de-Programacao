
# 🔁 **Repetição na Programação – O Computador Aprendendo a Fazer Algo Várias Vezes**

---

## 👶 Imagine o seguinte...

Você quer ouvir sua música favorita 3 vezes. Você pode:

❌ Fazer isso manualmente:  
> Dar play, esperar acabar, dar play de novo...

✅ Ou dizer pro celular:  
> **"Toque essa música 3 vezes!"**

**👉 Isso é repetição!**  
Você **manda o computador repetir uma tarefa**, e ele faz sozinho, sem que você precise repetir os comandos um por um.

---

## 🧠 O que é estrutura de repetição?

É quando o computador **repete uma ação várias vezes**, **automaticamente**.

Ele só para quando:
- Termina o número de repetições
- Ou uma **condição** diz: “agora pode parar”

---

## 📌 Temos 3 tipos:

---

### 1️⃣ **PARA** – Quando **sabemos quantas vezes** repetir

💬 Exemplo do dia a dia:  
> “Quero que você diga ‘Bom dia’ 5 vezes.”

👨‍🏫 Em pseudocódigo:
```plaintext
Para i de 1 até 5 faça
    Escreva("Bom dia!")
FimPara
```

🧠 Isso faz:
```
Bom dia!
Bom dia!
Bom dia!
Bom dia!
Bom dia!
```

---

### 2️⃣ **ENQUANTO** – Quando **não sabemos quantas vezes**, mas queremos **repetir até que algo aconteça**

💬 Exemplo do dia a dia:  
> “Enquanto eu estiver com fome, eu vou comer.”

👨‍🏫 Em pseudocódigo:
```plaintext
fome <- verdadeiro

Enquanto (fome == verdadeiro) faça
    Escreva("Comendo... 🍔")
    fome <- falso  // Aqui fingimos que a fome acabou
FimEnquanto
```

🧠 Isso faz:
```
Comendo... 🍔
```

---

### 3️⃣ **REPITA ATÉ** – Faz **pelo menos 1 vez** e **para quando a condição for verdadeira**

💬 Exemplo do dia a dia:  
> “Repita a senha até digitar certo.”

👨‍🏫 Em pseudocódigo:
```plaintext
senha <- ""

Repita
    Escreva("Digite a senha:")
    Leia(senha)
Até (senha == "1234")

Escreva("Senha correta! ✅")
```

🧠 Isso pode fazer:
```
Digite a senha:
> 0000  
Digite a senha:
> 1111  
Digite a senha:
> 1234  
Senha correta! ✅
```

---

## 🤯 Dúvidas comuns:

> ❓“Professor, por que não escrever 5 vezes o mesmo comando?”

Porque com repetição o computador **trabalha por você!**  
Se quiser repetir 100, 1000, 1 milhão de vezes... você não precisa escrever tudo!

---

## 🎓 Exemplo fácil com frutas:

> Você tem 4 maçãs e quer imprimir o nome de cada uma:

```plaintext
Para i de 1 até 4 faça
    Escreva("Maçã ", i)
FimPara
```

🧠 Saída:
```
Maçã 1
Maçã 2
Maçã 3
Maçã 4
```
---

## 👩‍🏫 Dica da Profê:

> “Toda repetição é como dizer: **continue fazendo isso até que eu diga para parar.**”
---

## 🎒 Atividade prática para sala:

**Situação:**
> Um aluno quer estudar 3 matérias. Crie uma repetição para mostrar o nome de cada uma.

```plaintext
Para i de 1 até 3 faça
    Leia(materia)
    Escreva("Estudando a matéria: ", materia)
FimPara
```

