Guia Prático: GitHub e Pull Requests 

 
Como criar sua conta no GitHub 

Acesse o site oficial: https://github.com. 
Clique em Sign up para se registrar. 
Preencha as informações solicitadas: e-mail, senha e nome de usuário. 
Confirme seu e-mail através do link enviado pela plataforma. 
Pronto! Sua conta estará ativa. 

 
Como criar um repositório remoto 

Depois de fazer login, clique no ícone de + no canto superior direito e selecione New repository. 
Preencha os seguintes campos: 
Nome do repositório: Exemplo — ola-mundo. 
Descrição: Opcional. 

Escolha se será público ou privado. 
Marque a opção Add a README file para já começar com um arquivo inicial. 
Clique em Create repository. 

 

Como clonar, enviar (push) e atualizar (pull) o repositório 

Para clonar o repositório (copiar para seu computador):
git clone https://github.com/SEU_USUARIO/ola-mundo.git 
cd ola-mundo 
 

Para enviar suas alterações locais para o GitHub (push): 

git add . 
git commit -m "mensagem explicando a alteração" 
git push origin main 
 

Para baixar atualizações do repositório remoto (pull): 

git pull origin main 
 
Exemplo Prático: Pull Request e Revisão de Código 

Como criar o arquivo principal 

Crie um novo arquivo com o seguinte conteúdo: 
echo 'print("Olá, mundo!")' > app.py 

Salvar e enviar esse arquivo para o repositório 


git add . 
git commit -m "Criação do script inicial com mensagem Olá, mundo" 
git push origin main 
 

Como criar uma nova branch para adicionar uma funcionalidade 

git checkout -b nova-mensagem 

 
Alterar o código do arquivo app.py 

Edite o arquivo para adicionar mais uma linha: 

print("Olá, mundo!") 
print("Bem-vindo ao GitHub!") 

Salvar e enviar essa alteração para a nova branch 

git add app.py 
git commit -m "Inclui nova mensagem de boas-vindas" 
git push origin nova-mensagem 
 
Criar um Pull Request (PR) 

Acesse seu repositório no GitHub. 
O site deve sugerir a criação de um Pull Request para o novo branch. 
Clique em Compare & pull request. 
Preencha o título e a descrição do que foi feito. 
Clique em Create pull request. 

Revisar o código (feito por um colaborador) 

O revisor pode deixar comentários específicos em trechos do código. 
Ele pode aprovar ou pedir ajustes. 
Quando tudo estiver certo, clique em Merge pull request e depois em Confirm merge.
Você pode também remover o branch clicando em Delete branch. 

Como atualizar sua branch principal (main) após o merge 

git checkout main 
git pull origin main 