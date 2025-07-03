# 🧠 Introdução ao Git
[GIT: Minicurso para Você Sair do Zero! (Aprenda em 45 Minutos)](https://www.youtube.com/watch?v=ts-H3W1uLMM)


O **Git** é um sistema de controle de versão distribuído que permite acompanhar o histórico de alterações de arquivos em projetos, colaborar com outras pessoas e manter diferentes versões do mesmo código de forma organizada e segura.  

Um **repositório (repo)** é onde todo o seu projeto fica armazenado, incluindo os arquivos do projeto e o histórico de alterações. Existem dois tipos de repositórios:
- **Repositório local**: está na sua máquina.
- **Repositório remoto**: está hospedado na nuvem (como no GitHub).

Uma **branch** (ramo) permite criar versões paralelas do projeto. A branch principal costuma se chamar `main` ou `master`. Você pode criar outras branches para desenvolver funcionalidades ou corrigir erros sem afetar o código principal.

Um **commit** é como uma fotografia do seu projeto em determinado momento. Ele registra todas as alterações que você preparou (adicionou ao "stage") com uma mensagem explicativa, ajudando a entender a evolução do projeto ao longo do tempo.

A **staging area** (ou área de preparação) é uma etapa intermediária entre editar arquivos e criar um commit. Quando você usa `git add`, os arquivos modificados são enviados para o **stage**, o que significa que eles estão prontos para serem incluídos no próximo commit. Isso permite que você selecione com cuidado quais alterações quer salvar no histórico, em vez de registrar todas as mudanças de uma vez.


O fluxo básico de trabalho com Git geralmente segue esta sequência:
1. Criar ou clonar um repositório.
2. Fazer alterações no projeto.
3. Adicionar os arquivos modificados ao **stage** com `git add`.
4. Criar um **commit** com `git commit`.
5. Enviar as alterações para o repositório remoto com `git push`.

Com o Git, você também pode **buscar** (`git fetch`) e **atualizar** (`git pull`) as alterações feitas por outras pessoas em um repositório remoto.

---

# 📘 Comandos Básicos do Git

## 📁 Repositório

Um repositório (**repo**) é onde o Git armazena seu projeto e o histórico de versões.

---

## 🔧 Inicializar Repositório

Inicia um novo repositório Git local.

```bash
git init
````

---

## 🌐 Adicionar Repositório Remoto

Conecta seu repositório local a um repositório remoto (como o GitHub).

```bash
git remote add origin <link-do-repositorio>
```

---

## 🔍 Verificar Status dos Arquivos

Exibe os arquivos modificados e os que estão no stage.

```bash
git status
```

---

## ➕ Adicionar Arquivos ao Stage

Adiciona arquivos modificados, criados ou deletados ao stage (prontos para commit).

```bash
git add <nome-do-arquivo>
```

---

## ↩️ Remover Arquivos do Stage

Remove arquivos do stage, retornando ao estado modificado.

```bash
git restore --staged <nome-do-arquivo>
```

---

## 📝 Criar um Commit

Cria um commit com os arquivos que estão no stage.

```bash
git commit --message "Descrição das alterações"
```

---

## 🔀 Renomear a Branch Atual para `main`

Muda o nome da branch padrão de `master` para `main`.

```bash
git branch -m main
```

---

## 📥 Clonar um Repositório

Faz o download de um repositório remoto para sua máquina.

```bash
git clone <link-do-repositorio>
```

---

## 🔄 Buscar Atualizações (fetch)

Busca atualizações do repositório remoto, sem alterar seus arquivos locais.

```bash
git fetch
```

---

## ⬇️ Baixar Atualizações (pull)

Baixa e aplica as atualizações do repositório remoto na sua máquina.

```bash
git pull origin main
```

---

## ⬆️ Enviar Commits para o Repositório Remoto

Envia seus commits locais para o repositório remoto.

```bash
git push origin main
```

---

## 📜 Ver Histórico de Commits

Exibe o histórico de commits do repositório.

```bash
git log
```
