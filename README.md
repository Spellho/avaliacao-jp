# avaliacao-jp

COMANDOS GIT:

1: git --version
--Mostra a versão do git instalada

2: git config --global user.name "---"
--Configura o nome de usuário do git local

3: git config --global user.email "---@-.-"
--Configura o email do git local

4: ls -la ~/.ssh
--Verifica se existe chave ssh

5: ssh-keygen -t ed25519 -C "---@-.-"
--Adiciona uma nova chave ssh

6: eval "$(ssh-agent -s)"
--Inicializa um agente-ssh

7: ssh-add ~/.ssh/id_ed25519
--Adiciona uma chave ssh ao agente

8:  clip < ~/.ssh/id_ed25519.pub
--Copia a chave ssh

9: ssh -T git@github.com
--Testa a conexão com o github

10: git init
--Inicializa um novo repositório git

11: git status
--Mostra o estado atual do repositório (arquivos modificados, novos arquivos e arquivos preparados para commit)

12: git add <filename ou .>
--Adiciona os arquivos ao índice para o próximo commit

13: git rm --cached <file> / git restore --staged <filename ou .>
--Remove os arquivos do indíce

14: git branch
--Lista todos os branchs locais (adicione -r ou -a no final para listar somente as branchs remotas ou todas as branchs respectivamente)

15: git checkout <branchname>
--Muda para a branch especificada

16: git checkout <previous-branchname>
--Volta à branch anterior

17: git checkout -b <branchname>
--Cria uma nova branch e muda para ela

18: git checkout -D <branchname>
--Deleta a branch especificada

19: git commit -m "<description>"
--Faz um commit com uma descrição

20: git reset --soft HEAD~1
--Desfaz o último commit mas mantém as mudanças no índice

21: git reset --hard HEAD~1
--Desfaz o último commit e as mudanças do índice

22: git merge <branch>
--Merge a branch atual na branch informada

23: git push
--Envia os commits do repositório atual para o remoto

24: git revert <commit-hash>
--Cria um novo commit que desfaz as mudanças do commit especificado

25: git branch -D <branchname>
--Deleta a branch especificada

26: git fetch
--Atualiza o repositório local com informações do repositório remoto sem mesclar

27: git pull
--Atualiza o repositório local com informações do repositório remoto e mescla com a branch atual

28: git reset --hard <commit-hash>
--Reverte a branch atual para como ela estava antes do pull

29: git clone "url ssh"
--Baixa o repositório correspondente à url ssh na máquina atual