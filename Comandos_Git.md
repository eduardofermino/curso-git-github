# Comandos Git

Guia de referência para os principais comandos de versionamento de código com Git.

---

## Lista de Comandos

| Comando | Descrição |
| :--- | :--- |
| `git status` | Mostra a branch atual, se não há commits, arquivos que não foram adicionados e o que está para commit |
| `git add <arquivo>` | Prepara o arquivo para versionamento (Staging Area) |
| `git reset <arquivo>` | Tira o arquivo do commit (descarta do Staging Area) |
| `git commit -m "mensagem"` | Commita as alterações preparadas |
| `git log` | Historico de todos os commits |
| `git diff` | Estado atual x estado do commit anterior de um arquivo |
| `git checkout -b <nome_branch>` | Cria uma branch e começa a usá-la |
| `git checkout <nome_branch>` | Muda de branch |
| `git branch` | Mostra todas as branches e indica a atual |
| `git merge <nome_branch>` | Faz o merge da branch selecionada com a atual |
| `git branch -D <nome_branch>` | Deleta a branch especificada |
| `git remote add origin <url>` | Vincula o repositório local com o remoto |
| `git branch -M <nome>` | Força a renomeação da branch atual |
| `git push origin main` | Envia todas as alterações da branch `main` local para o `origin` (repositório remoto) |
| `git pull origin main` | Atualiza a branch local atual com todas as alterações da branch `main` remota |
| `git clone <url_do_repositorio>` | Clona um repositório remoto para a sua máquina local |
| `git fetch` | Baixa novas branches e commits para o repositório local, nao altera o código atual **dica: é possível usar git checkout + nome da branch remota para clonar o cõdigo localmente** |