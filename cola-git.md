# 📚 Cola Git 
---

# 🔍 Verificar estado do projeto

```bash id="o3h2j1"
git status
```

Mostra:

* arquivos modificados
* arquivos novos
* staged
* branch atual

---

# ➕ Adicionar arquivos para commit

## Adicionar tudo

```bash id="v4m2q8"
git add .
```

👉 Coloca TODOS os arquivos modificados/staged para o próximo commit.

---

## Adicionar arquivo específico

```bash id="l7c1f9"
git add arquivo.java
```

---

# 💾 Criar commit

```bash id="s9d0k2"
git commit -m "fix: corrigindo configuração maven"
```

👉 Salva um “snapshot” do projeto.

---

# 🚀 Enviar para GitHub

```bash id="q5n8r4"
git push
```

👉 Envia commits locais para o repositório remoto.

---

# ⬇️ Atualizar projeto local

```bash id="m1z6x7"
git pull
```

👉 Baixa alterações do GitHub.

---

# 🌱 Trabalhando com branches

## Criar branch e entrar nela

```bash id="t8w3y6"
git checkout -b nome-da-branch
```

Exemplo:

```bash id="u2p9e5"
git checkout -b testes-javafx
```

---

## Ver branches

```bash id="g6h4v2"
git branch
```

A branch atual aparece com `*`.

---

## Trocar de branch

```bash id="y7r2n1"
git checkout master
```

OU:

```bash id="d3f8m0"
git checkout nome-da-branch
```

---

# 🔀 Juntar branch na master

## Entrar na master

```bash id="a9l5k3"
git checkout master
```

---

## Fazer merge

```bash id="f1t7q9"
git merge nome-da-branch
```

---

# ❌ Apagar branch

```bash id="p6j4w8"
git branch -D nome-da-branch
```

---

# ↩️ Descartar alterações

## Restaurar UM arquivo

```bash id="n4s2x5"
git restore arquivo.java
```

---

## Restaurar TUDO

```bash id="k8c1v7"
git restore .
```

👉 Volta tudo para o último commit.

---

# 📜 Ver histórico de commits

## Histórico resumido

```bash id="r3m7b1"
git log --oneline
```

---

## Histórico completo

```bash id="w9x5q2"
git log
```

---

# 🔍 Ver diferenças

```bash id="c2v8n6"
git diff
```

👉 Mostra linhas alteradas antes do commit.

---

# ⚙️ Configuração inicial Git

## Nome

```bash id="j7p4s9"
git config --global user.name "Seu Nome"
```

---

## Email

```bash id="h5d2l8"
git config --global user.email "seuemail@gmail.com"
```

---

## Ver configurações

```bash id="b1f6k3"
git config --list
```

---

# 🔐 Testar conexão GitHub SSH

```bash id="m8q3x1"
ssh -T git@github.com
```

---

# 📁 Fluxo padrão do dia a dia

```bash id="v7n2m5"
git status
git add .
git commit -m "mensagem"
git push
```

---

# 🧠 Filosofia do Git

## Arquivo alterado

Você mudou algo.

↓

## `git add`

Você escolheu o que vai entrar no commit.

↓

## `git commit`

Git salva um snapshot.

↓

## `git push`

Envia pro GitHub.

---

# 🧹 `.gitignore` recomendado

```gitignore id="x4z9c7"
.idea/
target/
out/
*.iml
```

👉 Evita subir lixo da IDE/build.

---

# 🏷️ Padrão profissional de commits

## Feature nova

```bash id="q2w8e4"
feat: adiciona sistema de login
```

---

## Correção

```bash id="n7r5t1"
fix: corrige erro no JavaFX
```

---

## Refatoração

```bash id="p4k9m2"
refactor: reorganiza estrutura do projeto
```

---

## Documentação

```bash id="d6s3v8"
docs: atualiza README
```

---

# 🛠️ Comandos Linux úteis para Git

## Ver pasta atual

```bash id="u5c1n7"
pwd
```

---

## Ver arquivos

```bash id="l9f4k2"
ls
```

---

## Entrar em pasta

```bash id="a3m8v6"
cd nome-da-pasta
```

---

# 🚨 Regras IMPORTANTES

✅ Sempre:

```bash id="r1x6z4"
git status
```

antes de commitar.

---

✅ Use branch para testes.

---

✅ Faça commits pequenos e descritivos.

---

✅ Não suba:

* `.idea`
* `target`
* `out`

---
