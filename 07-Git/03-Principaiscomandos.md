Aqui está uma versão em Markdown que detalha os principais comandos do Git e suas utilidades:

```markdown
# Principais Comandos do Git e Suas Utilidades

## 1. Git clone
- **Utilidade:** Baixar uma cópia do código-fonte de um repositório remoto (como GitHub) para seu computador local.
- **Uso comum:**
  ```bash
  git clone https://link-do-repositorio.git
  ```

## 2. Git branch
- **Utilidade:** Gerenciar ramificações (branches), permitindo que múltiplos desenvolvedores trabalhem simultaneamente em diferentes aspectos de um projeto.
- **Comandos:**
  - **Criação:**
    ```bash
    git branch nome-da-branch
    ```
  - **Listagem:**
    ```bash
    git branch
    git branch --list
    ```
  - **Exclusão:**
    ```bash
    git branch -d nome-da-branch
    ```

## 3. Git checkout
- **Utilidade:** Trocar de uma branch para outra, ou restaurar arquivos do repositório.
- **Uso:**
  - **Troca de branch:**
    ```bash
    git checkout nome-da-branch
    ```
  - **Criar e trocar imediatamente:**
    ```bash
    git checkout -b nome-da-branch
    ```

## 4. Git status
- **Utilidade:** Exibir o estado da branch atual, incluindo mudanças que precisam ser commitadas ou arquivos que não estão sendo rastreados.
- **Uso:**
  ```bash
  git status
  ```

## 5. Git add
- **Utilidade:** Adicionar alterações de arquivos ao próximo commit, colocando-os na área de staging.
- **Uso:**
  - **Adicionar um arquivo:**
    ```bash
    git add arquivo
    ```
  - **Adicionar todos os arquivos:**
    ```bash
    git add -A
    ```

## 6. Git commit
- **Utilidade:** Salvar as mudanças feitas no repositório local, estabelecendo um ponto que pode ser referenciado posteriormente.
- **Uso:**
  ```bash
  git commit -m "mensagem do commit"
  ```

## 7. Git push
- **Utilidade:** Enviar commits do repositório local para um repositório remoto.
- **Uso:**
  ```bash
  git push repositório-remoto nome-da-branch
  ```
  - **Estabelecer um rastreamento upstream para novas branches:**
    ```bash
    git push -u origin nome-da-branch
    ```

## 8. Git pull
- **Utilidade:** Atualizar o repositório local com as mais recentes mudanças do repositório remoto.
- **Uso:**

  ```bash
  git pull repositório-remoto
  ```

## 9. Git revert
- **Utilidade:** Desfazer mudanças feitas em commits anteriores, sem alterar o histórico de commits.
- **Uso:**

  ```bash
  git revert hash-do-commit
  ```

## 10. Git merge
- **Utilidade:** Unir mudanças de uma branch para outra, frequentemente usada para incorporar desenvolvimentos concluídos de uma branch de recursos para a branch principal.
- **Uso:**
  1. **Trocar para a branch destino:**
     
     ```bash
     git checkout branch-destino
     ```

  2. **Atualizar a branch destino:**

     ```bash
     git fetch
     ```

  3. **Fazer o merge:**

     ```bash
     git merge nome-da-branch-com-o-recurso
     ```
     
     Estes comandos são fundamentais para a interação diária com o Git, permitindo que desenvolvedores gerenciem eficazmente as versões de seus códigos e colaborem em projetos compartilhados.