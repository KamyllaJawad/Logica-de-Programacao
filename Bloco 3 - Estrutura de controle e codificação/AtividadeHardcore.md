## 🧩 **Desafio Guiado – Sistema de Cadastro de Produtos em Portugol**

### 🛒 Situação:

Você vai criar no **Portugol WebStudio** um sistema simples para **ajudar uma loja de eletrônicos a organizar seus produtos**. O sistema vai funcionar em formato de **menu interativo**, onde o usuário pode escolher o que deseja fazer: **cadastrar**, **visualizar**, **alterar**, **remover produtos**, ou **encerrar** o programa.

---

### 🎯 Objetivo:

Criar um sistema que:

1. Cadastre até 10 produtos (com nome, código, preço, quantidade e disponibilidade).
2. Mostre todos os produtos cadastrados.
3. Permita alterar os dados de um produto já registrado.
4. Remova um produto do sistema.
5. Calcule o valor total em estoque de cada produto.

---

### 🛠️ Como montar o programa passo a passo:

#### **PASSO 1 – Criar os vetores (listas) para guardar os dados dos produtos**
- Use 5 vetores:
  - Um para os códigos (`inteiro`)
  - Um para os nomes (`cadeia`)
  - Um para os preços (`real`)
  - Um para as quantidades (`inteiro`)
  - Um para a disponibilidade (`logico`)
- Crie também um contador chamado `totalProdutos` que começa em 0.

```portugol
inteiro codigos[10], quantidades[10]
real precos[10]
cadeia nomes[10]
logico disponiveis[10]
inteiro totalProdutos = 0
```

---

#### **PASSO 2 – Criar um menu de opções dentro de um `faca ... enquanto`**
- O menu deve repetir até o usuário escolher sair.
- Mostre as opções:
  - `1 - Cadastrar`
  - `2 - Listar`
  - `3 - Alterar`
  - `4 - Remover`
  - `5 - Sair`
- Use `escolha ... caso` para controlar cada opção.

---

#### **PASSO 3 – Cadastrar Produto**
- Verifique se ainda não atingiu o limite de 10 produtos.
- Peça:
  - Código
  - Nome
  - Preço
  - Quantidade
  - Se está disponível (1 para sim, 0 para não)
- Armazene os dados nas posições correspondentes do vetor.
- Ao final, **aumente `totalProdutos` em 1**.

---

#### **PASSO 4 – Listar Produtos**
- Verifique se `totalProdutos` é maior que zero.
- Use um laço `para` para mostrar todos os dados cadastrados.
- Multiplique `preço * quantidade` para mostrar o valor total no estoque do produto.

---

#### **PASSO 5 – Alterar Produto**
- Peça ao usuário o **código** do produto que deseja alterar.
- Procure esse código no vetor.
- Se encontrar, peça os novos dados (nome, preço, quantidade, disponibilidade).
- Substitua os dados antigos pelos novos.
- Se não encontrar, mostre uma mensagem de erro.

---

#### **PASSO 6 – Remover Produto**
- Peça o código do produto a remover.
- Encontre a posição do produto.
- Se existir, **desloque todos os dados que estão abaixo para cima**, “apagando” o produto.
- Diminua `totalProdutos` em 1.

---

### ⚠️ Regras importantes:
- Use `se`, `senao`, `para`, `faca enquanto`, `escolha caso` corretamente.
- Sempre verifique se o produto existe antes de alterar ou excluir.
- Organize bem as mensagens para que o usuário entenda o que fazer.

---

### 💡 Dica Final:

Pense no programa como se fosse uma **caixa registradora** que guarda uma lista de produtos e te deixa ver, mudar ou excluir o que quiser.  
Faça **um passo de cada vez** e **teste sempre** após terminar cada função do menu.
