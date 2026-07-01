# Prática de Git - Repositório Compartilhado

## Objetivo

O objetivo desta atividade é praticar os principais comandos do Git utilizando um único repositório compartilhado.

Ao final da atividade, cada aluno deverá ter realizado operações de:

- Clonar um repositório
- Criar branch
- Fazer alterações
- Adicionar arquivos
- Criar commits
- Enviar alterações para o GitHub
- Atualizar o repositório local
- Resolver conflitos simples
- Criar Pull Request
- Fazer merge

---

# Etapa 1 - Clonar o repositório

Clone o repositório fornecido.

```bash
git clone <URL_DO_REPOSITORIO>
```

Entre na pasta do projeto.

```bash
cd nome-do-repositorio
```

---

# Etapa 2 - Verificar o status

Confira a situação do repositório.

```bash
git status
```

Veja o histórico.

```bash
git log --oneline
```

Veja as branches existentes.

```bash
git branch
```

---

# Etapa 3 - Criar uma branch

Cada aluno deverá criar uma branch com seu nome.

Exemplo:

```bash
git checkout -b aluno-joao
```

ou

```bash
git switch -c aluno-joao
```

---

# Etapa 4 - Criar sua pasta

Na raiz do projeto, crie uma pasta com seu nome.

Exemplo:

```
/
├── joao/
```

---

# Etapa 5 - Criar um arquivo

Dentro da sua pasta, crie um arquivo chamado:

```
MEU_DADOS.md
```

Com o seguinte conteúdo:

```markdown
# João

## Informações

- Nome:
- Cidade:
- Hobby favorito:

```

---

# Etapa 6 - Verificar alterações

```bash
git status
```

---

# Etapa 7 - Adicionar arquivos

Adicionar apenas sua pasta.

```bash
git add joao/
```

ou adicionar tudo.

```bash
git add .
```

---

# Etapa 8 - Criar um commit

Exemplo:

```bash
git commit -m "Adiciona pasta do João"
```

---

# Etapa 9 - Enviar para o GitHub

```bash
git push origin aluno-joao
```

---

# Etapa 10 - Criar Pull Request

No GitHub:

- Compare sua branch
- Crie um Pull Request
- Aguarde aprovação

---

# Etapa 11 - Atualizar a branch principal

Após o merge realizado pelo professor:

```bash
git checkout main
```

```bash
git pull origin main
```

---

# Etapa 12 - Criar um conflito

Todos deverão editar o mesmo arquivo:

```
alunos.txt
```

Cada aluno deverá adicionar seu nome na última linha.

Exemplo:

```
Ana
Carlos
Maria
Pedro
```

Faça novamente:

```bash
git add .
```

```bash
git commit -m "Adiciona meu nome na lista"
```

```bash
git push
```

Caso outro aluno tenha enviado antes:

```bash
git pull origin main
```

Resolva o conflito.

Depois:

```bash
git add .
```

```bash
git commit
```

```bash
git push
```

---

# Etapa 13 - Histórico

Visualize o histórico.

```bash
git log --oneline --graph --all
```

---

# Etapa 14 - Diferenças

Veja as diferenças do último commit.

```bash
git diff
```

ou

```bash
git diff HEAD~1
```

---

# Etapa 15 - Remover um arquivo

Crie um arquivo temporário.

```bash
touch teste.txt
```

Faça commit.

Depois remova.

```bash
git rm teste.txt
```

Commit novamente.

---

# Etapa 16 - Desfazer alterações

Descartar alterações em um arquivo.

```bash
git restore arquivo.txt
```

Remover arquivo da área de staging.

```bash
git restore --staged arquivo.txt
```

---

# Etapa 17 - Verificar remoto

```bash
git remote -v
```

---

# Etapa 18 - Limpar branches locais

Após o merge:

```bash
git checkout main
```

```bash
git pull
```

Excluir sua branch local.

```bash
git branch -d aluno-joao
```

---

# Comandos praticados

- git clone
- git status
- git log
- git branch
- git checkout
- git switch
- git add
- git commit
- git push
- git pull
- git diff
- git rm
- git restore
- git remote
- git merge
- git branch -d

---

# Desafio Extra ⭐

1. Criar uma nova branch.
2. Adicionar uma imagem na sua pasta.
3. Editar o README principal do projeto.
4. Resolver um conflito sem ajuda.
5. Criar dois commits e depois uni-los utilizando **git rebase -i**.
6. Explicar para a turma quando utilizar:
   - `git merge`
   - `git rebase`
   - `git stash`
   - `git cherry-pick`

---
