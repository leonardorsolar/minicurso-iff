# Criar uma Conta do Github

Fase 1 Como criar um conta no github:
Passo 1: Acesse o site do github: https://docs.github.com/pt
Passo 2: Vá em Get started>introdução>guia de início rápido
Passo 3: Clique em Criar uma conta no GitHub
Passo 4: Crie a sua conta

# Tutorial de como criar um repositório no github:

Passo 1: Acesse o site do github: https://docs.github.com/pt
Passo 2: Vá em Get started>introdução>guia de início rápido
Passo 3: Clique em Olá, Mundo

Fase 1 Criar um repositório no github:
Passo 1: Acesse a sua conta do github:
Passo 2: No canto superior direito de qualquer página, selecione e clique em Novo repositório.
Passo 3: Na caixa "Nome do repositório", digite front-form.
Passo 4: Na caixa "Descrição", digite uma breve descrição. Por exemplo, digite "Este repositório é para praticar html, css e javascript”.
Passo 5: Selecione se o repositório será Público
Passo 6: Clique em Criar repositório.

Fase 2 Versione o código no git:
Passo 1: crie a pasta MINICURSO e depois crie a pasta front e depois a pasta front-form em documentos
Passo 2: Acesse a pasta e na barra de endereço digite: cmd
Passo 3: No cmd digite:
echo "# front-form" >> README.md
Passo 4: No cmd digite: git init
Passo 5: No cmd digite: git status
Passo 6: No cmd digite: git add .

Fase 3 configurações do git:
Passo 1: No cmd digite: git commit -m "first commit"
Passo 2: No cmd digite: git config --global user.name "Seu Nome"
ex.: git config --global user.name leonardosolar
Passo 3: No cmd digite: git config --global user.email "seu.email@example.com"
ex.: git config --global user.email leonardos@yahoo.com

Fase 4 Commit no git:
Passo 1: No cmd digite: git commit -m "first commit"
Passo 2: No cmd digite: git status

Fase 5 Criar a brach:
Passo 1: No cmd digite: git branch -M main
Passo 2: No cmd digite: git status

Fase 6 Criar o acesso remoto:
Passo 1: No cmd digite:
git remote add origin https://github.com/leonardorsolar/front-form.git

Fase 7 Autorizando o push:
Passo 1: No cmd digite: git push -u origin main
Passo 2: entre na conta para autorização: Sign in to GitHub
Passo 3: clique em autorizar:

Fase 8 visualizando o repositório:
Passo 1:Dê um reload na página no github

Fase 8 visualizando o projeto no vscode
Passo 1: abra a pasta(folder) front-form no Vscode

Fase 8 Modificando o arquivo:
Passo 1: modificando o arquivo: dentro do arquivo README.md, digite: # Minicurso
Passo 2: visualizando a modificação: dentro do cmd digite: git status
Passo 3: Adicionando ao stage: dentro do cmd digite: git add .
Passo 4: visualizando a modificação: dentro do cmd digite: git status
Passo 5: Adicionando ao stage: dentro do cmd digite: git commit -m"Inserindo um título"
Passo 6: visualizando a modificação: dentro do cmd digite: git status
Passo 7: Dê um reload na página no github
