# Guia Prático: GitHub e Pull Requests

## Como criar sua conta no GitHub

1. Acesse o site oficial: https://github.com  
2. Clique em **Sign up** para se registrar  
3. Preencha as informações solicitadas: e-mail, senha e nome de usuário  
4. Confirme seu e-mail através do link enviado pela plataforma  
5. Pronto! Sua conta estará ativa  

---

## Como criar um repositório remoto

1. Faça login na sua conta  
2. Clique no ícone de **+** no canto superior direito e selecione **New repository**  
3. Preencha os campos:
   - Nome do repositório: exemplo — `ola-mundo`
   - Descrição: opcional
   - Visibilidade: público ou privado
   - Marque a opção **Add a README file**  
4. Clique em **Create repository**

---

## Como clonar, enviar (push) e atualizar (pull) o repositório

### Clonar o repositório:

```bash
git clone https://github.com/SEU_USUARIO/ola-mundo.git
cd ola-mundo
```

### Enviar suas alterações (push):

```bash
git add .
git commit -m "mensagem explicando a alteração"
git push origin main
```

### Atualizar com alterações do remoto (pull):

```bash
git pull origin main
```

---

## Exemplo Prático: Pull Request e Revisão de Código

### Criar o arquivo principal:

```bash
echo 'print("Olá, mundo!")' > app.py
```

### Salvar e enviar esse arquivo para o repositório:

```bash
git add .
git commit -m "Criação do script inicial com mensagem Olá, mundo"
git push origin main
```

### Criar uma nova branch para funcionalidade:

```bash
git checkout -b nova-mensagem
```

### Alterar o conteúdo do arquivo `app.py`:

```python
print("Olá, mundo!")
print("Bem-vindo ao GitHub!")
```

### Salvar e enviar essa alteração para a nova branch:

```bash
git add app.py
git commit -m "Inclui nova mensagem de boas-vindas"
git push origin nova-mensagem
```

---

## Criar um Pull Request (PR)

1. Acesse o repositório no GitHub  
2. O site deve sugerir automaticamente a criação do Pull Request  
3. Clique em **Compare & pull request**  
4. Preencha o título e a descrição  
5. Clique em **Create pull request**

---

## Revisar o código (por um colaborador)

- O revisor pode comentar diretamente nas linhas do código  
- Pode aprovar ou solicitar modificações  
- Quando aprovado, clique em **Merge pull request** e depois em **Confirm merge**  
- Opcional: **Delete branch** para manter o repositório limpo

---

## Atualizar sua branch `main` após o merge

```bash
git checkout main
git pull origin main
```
