## 🔍 O que é Git?
Git é um sistema de controle de versão distribuído gratuito e de código aberto, projetado para lidar com tudo, desde projetos pequenos a muito grandes, com velocidade e eficiência.
Ele é um DVCS(Sistema de controle de versão distribuído), pois os arquivos do projeto são clonados em cada desktop;

## 🔍 O que é GitHub?
De forma simples, ele é o servidor que armazena os projetos utilizados pelo Git.

## ⌨ Comandos Principais
- ```git clone``` => Clona o projeto desejado no desktop atual;

- ```git clone URL --branch NOMEBRANCH --single-branch``` => Clona somente a branch indicada;

- ```git status``` => Verifica se há novos arquivos que ainda não estão no *stage in area*(É onde fica os arquivos/alterações que serão enviados no commit);

- ```git add``` => Coloca os arquivos selecionados no *stage in area*;

- ```git commit -m``` => Prepara as alterações do *stage in area* para enviar para o remoto;

- ```git pull``` => Busca as alterações do projeto que não estão na branch atual e mescla;

- ```git push``` => Envia as alterações para o remoto;

- ```git remote add origin LINK``` => Adiciona o servidor remoto que será enviado o projeto caso tenha sido criado localmente;

## ⚙ Comandos de Configuração
- ```git config --global user.name "NOME"``` => Altera o nome do autor das alterações no projeto;

- ```git config --global user.email email``` => Altera o e-mail do autor das alterações no projeto;

- ```git config --global init.defaultBranch NOME``` => Altera a branch inicial quando for criado um novo repositório local;

- ```git config --global credential.helper store``` => Seta as credenciais para ficarem salvas;

- ```git config --global credential.helper NOME``` => Usa a credencial indicada;

## 📑 Comandos Utilitários

- ```git config --global --show-origin credential.helper``` => Retorna o local do arquivo que está armazenada as credenciais;

- ```git config --global --list``` => Lista as configurações globais que foram setadas;

- ```git log``` => Retorna as informações dos commits até o momento, como: Autor, data, hash do commit, etc;

- ```git reflog``` => Retorna os commits e mostra onde está localizada cada branch nos commits;

- ```git remote -v``` => Visualizar o servidor que o projeto está vinculado;

- ```git commit -ammend -m"MENSAGEMCOMMIT"``` => Altera a mensagem do último commit;

- ```git reset --soft HASHCOMMIT``` => Pega os commits posteriores ao commit escolhido
e coloca no *stage in area*;

- ```git reset --mixed HASHCOMMIT``` => Pega os commits posteriores ao commit escolhido
e coloca fora do *stage in area*;

- ```git reset --hard HASHCOMMIT``` => Apaga os arquivos posteriores ao commit escolhido;

- ```git restore MENSAGEMCOMMIT``` => Restaura para o último commit;

- ```git reset CAMINHOARQUIVO``` => Retira um arquivo do *stage in area*;

- ```git restore --staged CAMINHOARQUIVO``` => Retira um arquivo do *stage in area*;