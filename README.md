## **Comandos Git**

### **Inicializando um repositório**
* **Criar um novo repositório Git**  
  `git init`  
  Inicializa um repositório Git vazio no diretório atual.

* **Configurar o branch principal como `main`**  
  `git branch -M main`  
  Renomeia a branch atual para `main`, que é o novo padrão de muitos repositórios.

* **Adicionar arquivos para o commit**  
  `git add .`  
  Adiciona todos os arquivos modificados para a área de staging (preparação para commit).

* **Fazer o primeiro commit**  
  `git commit -m "[mensagem]"`  
  Faz o commit das alterações adicionadas, com uma mensagem descritiva. Exemplo: `git commit -m "Primeiro commit"`

* **Adicionar repositório remoto**  
  `git remote add origin [link do repositório do GitHub]`  
  Conecta o repositório local a um repositório remoto, normalmente no GitHub.

* **Enviar alterações para o repositório remoto**  
  `git push origin main`  
  Envia as alterações locais para o repositório remoto no branch `main`.

---

### **Trabalhando com repositórios já existentes**

* **Adicionar repositório remoto**  
  `git remote add origin [link do repositório do GitHub]`  
  Conecta o repositório local a um repositório remoto, normalmente no GitHub.

* **Configurar o branch principal como `main`**  
  `git branch -M main`  
  Renomeia a branch atual para `main`.

* **Enviar alterações para o repositório remoto (primeiro push)**  
  `git push -u origin main`  
  Envia as alterações locais para o repositório remoto pela primeira vez, e associa o repositório local ao remoto.

---

### **Manutenção e updates**

* **Adicionar arquivos para o commit**  
  `git add .`  
  Adiciona todos os arquivos modificados para a área de staging.

* **Fazer commit das alterações**  
  `git commit -m "[mensagem]"`  
  Realiza o commit das alterações feitas, com uma descrição relevante (ex: `git commit -m "Corrige erro de cálculo"`).

* **Enviar alterações para o repositório remoto**  
  `git push origin main`  
  Envia as alterações locais para o repositório remoto.

---

### **Clonando um repositório**

* **Clonar repositório remoto**  
  `git clone [link do repositório do GitHub]`  
  Clona um repositório remoto para a sua máquina local.

---

### **Atualizando a versão local**

* **Puxar as últimas alterações do repositório remoto**  
  `git pull`  
  Baixa as alterações mais recentes do repositório remoto e as incorpora no repositório local.

---

### **Configurações via VS Code (ou terminal)**

* **Configurar o nome de usuário global do Git**  
  `git config --global user.name "[nome do usuário]"`  
  Define o nome de usuário global para os commits.

* **Configurar o e-mail global do Git**  
  `git config --global user.email "[e-mail]"`  
  Define o e-mail global para os commits.

---

### **Trabalhando com branches**

* **Criar uma nova branch**  
  `git branch [nome-da-branch]`  
  Cria uma nova branch.

* **Trocar para uma branch existente**  
  `git checkout [nome-da-branch]`  
  Muda para uma branch existente.

* **Criar e trocar para uma nova branch**  
  `git checkout -b [nome-da-branch]`  
  Cria uma nova branch e já muda para ela.

* **Excluir uma branch local**  
  `git branch -d [nome-da-branch]`  
  Exclui uma branch local. Use `-D` (letra maiúscula) para forçar a exclusão, mesmo que a branch tenha alterações não mescladas.

* **Mesclar uma branch na branch atual**  
  `git merge [nome-da-branch]`  
  Mescla as mudanças de uma branch específica para a branch atual.

---

### **Trabalhando com repositórios remotos**

* **Exibir repositórios remotos configurados**  
  `git remote -v`  
  Lista os repositórios remotos configurados e suas URLs.

* **Alterar URL de um repositório remoto**  
  `git remote set-url origin [nova-url]`  
  Altera a URL de origem do repositório remoto (por exemplo, para trocar de HTTPS para SSH).

* **Buscar atualizações do repositório remoto (sem aplicar)**  
  `git fetch`  
  Baixa as atualizações do repositório remoto, mas sem aplicá-las no repositório local.

* **Excluir uma branch remota**  
  `git push origin --delete [nome-da-branch]`  
  Exclui uma branch remota do repositório.

---

### **Comandos avançados e úteis**

* **Verificar status do repositório**  
  `git status`  
  Exibe o status atual do repositório, incluindo arquivos modificados e a branch ativa.

* **Visualizar o histórico de commits**  
  `git log`  
  Exibe o histórico de commits, mostrando detalhes como o autor, data e mensagem de commit.

* **Ver as diferenças entre o estado atual e o último commit**  
  `git diff`  
  Exibe as diferenças entre as modificações não comitadas e o último commit.

* **Reverter o último commit (sem alterar o código)**  
  `git revert HEAD`  
  Cria um novo commit que reverte o commit mais recente, sem afetar o código anterior.

* **Alterar a mensagem do último commit**  
  `git commit --amend`  
  Permite editar a mensagem do último commit. Use com cuidado para evitar problemas de reescrita do histórico.

* **Reverter alterações em um arquivo específico**  
  `git checkout -- [arquivo]`  
  Desfaz as alterações em um arquivo específico, revertendo-o para o estado do último commit.

* **Criar um stash para salvar alterações temporárias**  
  `git stash`  
  Salva temporariamente alterações não comitadas para permitir que você troque de branch ou realize outras tarefas.

* **Aplicar um stash salvo**  
  `git stash apply`  
  Restaura as mudanças salvas no último stash.

* **Excluir um stash específico**  
  `git stash drop [stash@{n}]`  
  Exclui um stash específico.

* **Ver os stashes salvos**  
  `git stash list`  
  Exibe a lista de todos os stashes salvos.
