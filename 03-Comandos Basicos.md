# Introdução aos Comandos Básicos do Git
O Git é uma ferramenta essencial no dia a dia de quem desenvolve software. Ele permite que você acompanhe as mudanças no código, trabalhe em equipe com mais segurança e até volte no tempo se algo der errado.

Abaixo, você encontra os comandos fundamentais para dar os primeiros passos com o Git, explicados de forma simples e direta:

## git init — Iniciando seu repositório
Esse é o primeiro comando que você vai usar. Com git init, você transforma qualquer pasta comum em um repositório Git. Isso significa que o Git vai começar a rastrear as mudanças feitas ali.
Execute esse comando dentro da pasta do seu projeto. O Git vai criar um diretório oculto chamado .git, onde guardará todo o histórico de alterações.

## git status — Verificando o que mudou
Depois de criar ou modificar arquivos, você pode usar git status para saber o que está acontecendo no seu repositório: quais arquivos foram alterados, quais ainda não estão sendo rastreados e o que está pronto para ser salvo.
Esse comando é ótimo para ter uma visão geral antes de continuar.

## git add — Preparando os arquivos para salvar
O comando git add serve para dizer ao Git: “Esses arquivos aqui estão prontos para serem salvos no próximo commit.” Isso é chamado de adicionar à área de staging.
Quer preparar todos os arquivos modificados de uma vez? Use: git add .

## git commit — Salvando suas mudanças
Depois de adicionar os arquivos com git add, é hora de realmente salvar as mudanças. Com git commit, você cria um ponto de restauração no seu projeto — é como tirar um "snapshot" com uma descrição do que foi feito.
<pre><code>git commit -m "Cria página inicial do site"</code></pre>
A mensagem entre aspas deve explicar de forma breve o que foi feito. Isso ajuda a entender o histórico do projeto no futuro (ou quando você trabalha com outras pessoas).

## git log — Visualizando o histórico
Quer saber tudo o que já foi feito no projeto? Use git log. Ele mostra uma lista com todos os commits, incluindo o autor, a data e a mensagem de cada um.

## Conclusão
Esses cinco comandos (git init, git status, git add, git commit e git log) formam a base para começar a usar o Git com segurança. Com eles, você pode:

- Iniciar o controle de versão do seu projeto;

- Verificar quais arquivos mudaram;

- Preparar e registrar mudanças;

- Acompanhar todo o histórico de desenvolvimento.

Com o tempo, você vai se familiarizar com outros comandos, como git branch, git merge e git push. Mas dominando esses primeiros, você já está pronto para trabalhar com o Git no seu dia a dia.
