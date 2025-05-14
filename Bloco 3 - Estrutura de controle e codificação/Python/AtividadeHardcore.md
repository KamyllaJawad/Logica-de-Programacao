## 🧩 Desafio 1 — Sistema de Cadastro na Biblioteca 📚

**História:**
Você está desenvolvendo um sistema de cadastro para a biblioteca da escola. Só podem se cadastrar:

* Alunos com **14 anos ou mais**
* Que **não estejam devendo livros**
* E cujo **nome tenha no máximo 12 letras** (o sistema não aceita nomes longos)

Além disso, se a idade estiver **entre 14 e 17**, deve ser exibido um aviso:
**"Cadastro de menor vinculado a um responsável."**

### Regras:

1. Solicite o `nome`, `idade`, e se está devendo livros (`sim` ou `não`).
2. Verifique:

   * Se a pessoa atende **todos os critérios**, mostre:
     ✅ `"Cadastro aprovado para [nome]!"`
     (e se for menor de idade, exiba o aviso do responsável)
   * Caso contrário, recuse e diga exatamente **qual regra foi quebrada**:

     * Se for muito jovem: `"Cadastro negado: idade insuficiente."`
     * Se estiver devendo: `"Cadastro negado: regularize sua dívida."`
     * Se o nome for longo: `"Cadastro negado: nome muito extenso."`

### O que será testado:

✅ `input()`, `if`, `elif`, `else`
✅ `len()`, operadores relacionais
✅ Combinações de múltiplas condições (`and`, `or`)
✅ Impressão personalizada com nome do usuário


---

## 🧠 Desafio 2 — **Desarme a Bomba com Códigos Múltiplos 💣**

### História:

Você foi trancado em uma sala com uma bomba. Para desarmá-la, você deve **descobrir uma sequência secreta de 3 códigos**.
Cada tentativa errada **consome uma chance**, e você só tem **5 chances no total**.

A sequência correta é:

* Primeiro código: `3`
* Segundo código: `1`
* Terceiro código: `4`

Mas atenção:

* Os códigos devem ser digitados **na ordem**.
* Se errar um código, o sistema reinicia a sequência e **perde 1 tentativa**.
* Se acertar todos os 3 na ordem certa, a bomba é desativada com a mensagem:
  ✅ `"Bomba desativada com sucesso!"`
* Se usar as 5 chances e não acertar, exiba:
  ❌ `"BOOM! Você falhou ao desativar a bomba."`

---

### Regras de implementação:

1. Use um `while` que permita no máximo 5 tentativas.
2. Dentro do loop:

   * Peça o primeiro código. Se errado, exiba `"Código incorreto!"` e continue o loop.
   * Se certo, vá para o segundo.
   * Repita o mesmo para o segundo e terceiro código.
   * Se errar qualquer um, reinicie do primeiro código e perca uma tentativa.
3. Se os três forem digitados corretamente, exiba a mensagem de sucesso e interrompa o jogo com `break`.

---

### O que será testado:

✅ Uso avançado de `while` com contador de tentativas
✅ Lógica de fluxo condicional aninhada
✅ Controle de erro e reinício de sequência
✅ Feedback imediato para o jogador
✅ `break` para encerrar o jogo antecipadamente

