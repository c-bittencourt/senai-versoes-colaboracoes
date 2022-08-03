# senai-versoes-colaboracoes
README.MD

Atividade Online e Encontro Remoto - PFS UC7 - Versionamento - 
Sequência de comandos usados para versionamento (Git)

Ações no repositório local
1. Foi criada pasta para versionamento no Windows Explorer (senai-versoes-colaboracoes)
2. Com o Git iniciado, o versionamento foi ativado para a pasta ("git init")
3. Foi criado o arquivo "versoes.txt"
4. Para verificação do status completo do repositório, foi rodado o comando "git status"
5. O arquivo criado foi então transferido para o staging, através do comando "git add."
6. Para verificar as alterações antes de salvar, foi usado novamente o comando "git status"
7. As alterações foram então salvas (git commit -m "meu primeiro commit")
8. Para verificar as alterações confirmadas no repositório, foi executado o comando "git log"
9. Usando o número do commit, foi visualizada a alteração no projeto ("git show <número do commit>.")

Ações no reposítório remoto (Github)
1. Após as configurações no repositório local, foi iniciada a configuração para publicação no repositório online informando a pasta remota (git remote add origin https://github.com/c-bittencourt/senai-versoes-colaboracoes)
2. Foi visualizado o repositório remoto ("git remote -v")
3. Em seguida, as alterações foram publicadas no repositório remoto ("git push -u origin master")
4. Por fim, o repositório publicado foi visualizado no navegador
5. Para simular também a configuração de arquivos que não desejamos publicar, foi criado o arquivo "arquivo-nao-publicado.txt" e, em seguida, o arquivo ".gitignore", usando depois o git status, o git add o git commit ("adicionando o gitignore") e o git push para sincronizar com o repositório remoto

Simulação de conflito
1. No repositório remoto, foi criado um arquivo README.MD
2. Após essa operação, a alteração foi baixada para o repositório local ("git pull")
3. Em seguida, foi criada uma ramificação ("git checkout -b tarefa/minha-primeira-branch")
4. O arquivo README.MD foi então editado e salvo. No Git Bash, nessa branch, foi usado o git add, o commit (git commit -m "adicionando o comando git status") e o "git push origin tarefa/minha-primeira-branch" para enviar a alteração na branch para o repositório remoto
5. Outra branch foi criada ("git checkout -b exemplo-branch"), o arquivo README.MD foi editado, foi usado o git add nessa branch, o git commit e o git push para a sincronização com o repositório remoto
6. Foi feita a mesclagem com a branch "minha-primeira-branch" ("git merge tarefa/minha-primeira-branch"), os conflitos foram identificados e editados e, em seguida, o arquivo foi enviado para staging, foi realizado o commit e finalmente publicado no repositório remoto
