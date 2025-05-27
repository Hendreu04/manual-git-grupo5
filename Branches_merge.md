O que são branches?

As branches são como ambientes separados dentro do repositório, onde é possível desenvolver recursos, testar novas funcionalidades de forma segura, sem afetar o ambiente principal (a branch main). As mudanças feitas dentro de uma outra branch (sem ser a main) ficam isoladas das mudanças feitas por outras pessoas da branch principal, isso permite que novas implementações e funcionalidades sejam feitas sem correr o risco de afetar o projeto.

Criar, mudar e deletar branches

O comando para criar uma branch no git é através do comando:
git branch [nome-da-branch]

Porém, é importante lembrar que ao criar uma branch, você permanece na sua branch atual. Para alterar da branch atual para a nova branch criada, você deve utilizar o comando:
git checkout [nome-da-branch]

Caso algo tenha dado errado e você precise deletar uma branch local, você deve utilizar o comando:
git branch -D [nome-da-branch]

Caso você precise deletar uma branch remota, utilize:
git push [nome-do-origin] [nome-da-branch] --delete