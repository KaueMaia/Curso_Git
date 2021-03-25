# Aprendendo usar o Git


## Aula 1

O que foi que eu aprendi aqui?

descubri o munndo do git

Explicamos o que é Git e GitHub

Conhecendo git e github - Luis Quesada

## Aula 2

O que foi que eu aprendi aqui?

aprendi os codigos basicos

Instalamos o Git e vimos alguns comandos

Comando visto: - Luis Quesada

- ls Lista o conteúdo de um diretório
- ls -a Lista os diretórios, arquivos oculto e executáveis
- pwd Mostra o diretório corrente
- cd [caminho] Muda de diretório
- cd .. Volta um diretório acima
- cd ~ Volta para seu diretório /home
- mkdir [pasta] Cria uma pasta com o nome desejado
- mkdir [pasta1] [pasta2] Cria pasta1 e pasta2 ao mesmo tempo
- mkdir 'Pasta Separada' Cria 1 única pasta com o nome Pasta Separada
- mkdir -p [pasta]/[sub-pasta] Cria um diretório e um sub-diretório
- rm -r [pasta/arquivo] Deleta uma pasta ou arquivo
- mv [velho] [novo] Renomear uma pasta ou arquivo
- mv [arquivo] [caminho] Move o arquivo para um determinado caminho
- cp [arquivo] [caminho] Copia um arquivo para um determinado caminho
- echo [mensagem] Exibe uma mensagem em seu shell
- cat Escreve no terminal (Ctrl+D em uma linha vazia para sair)
- cat > [arquivo] Escreve no terminal, cria arquivo e salva nele
- cat >> [arquivo] Escreve no terminal, salva no final do arquivo
- cat [arquivo] Mostra conteúdo do arquivo no terminal
- touch [arquivo] Cria um arquivo
- clear Limpa o terminal
- history Ver o histórico de comandos
- history [n] Ver os últimos comandos
- history -c Apagar o histórico
- git diff destaca as diferencias & modificaciones


## Aula 3

O que foi que eu aprendi aqui?

Configurando o GIT - Luis Quesada

Para iniciar um repositório local:
git init
Para ver o status do repositório local:
git status

Mudando o status de um arquivo:
Adicionando um arquivo para o Stage:
git add [arquivo] Adiciona arquivo específico
git add . Adiciona todos os arquivos
Retira arquivo do Stage:
git rm --cached [arquivo] Remove arquivo não rastreado do staged
git restore --staged [arquivo] Remove arquivo modificado do staged
git restore --staged .
Commita/Envia o Stage:
git commit -m '[Mensagem]' Commita com a Mensagem escolhida
git commit -am '[Mensagem]' Adiciona todos os arquivos modificados e
commita com a Mensagem escolhida

## Aula 4

O que foi que eu aprendi aqui?

Vendo histórico de commits: - Luis Quesada

git log
git log --pretty=oneline Organizar em 1 linha
git log --stat Mais informações
git log -p Ver as modificações
git log -p -2 Ver as 2 últimas modificações
git log --since=2.days Filtrar por tempo
git log --author='Kauê Maia' Filtrar por autor

Recuperar um ponto do histórico:
Voltando 1 commit:
git reset --soft HEAD~ Arquivos ficam no unstaged
git reset --hard HEAD~ Volta exatamente para o snapshot
Voltando para um commit específico:
git reset --soft [hash]
git reset --hard [hash]
Lembre de ver antes as diferenças:
git log --pretty=oneline -p -2

HEAD
git checkout HEAD~2 Voltando 2 commits
git checkout HEAD~~ Voltando 2 commits também
git checkout master Para voltar a nossa branch padrão
No comando git log vemos onde o HEAD está apontando:
git log --pretty=oneline


## Aula 5

O que foi que eu aprendi aqui?

Branch - Luis Quesada

Usando Branches:
Vendo os branches:
git branch
Criar uma branch:
git checkout -b [nome]
git checkout -b [nova] [antiga]
Mudar para outra branch:
git checkout [nome]
Para apagar um branch:
git branch -d [nome] 

Usando o Merge / fusão:

Usando o merge:
git merge [branch]
Forma interessante de ver:
git log --pretty=oneline --graph

Usando o Rebase:
git rebase [branch]
Dica para visualizar o log:
git log --pretty=oneline --graph

## Aula 6

O que foi que eu aprendi aqui?

Aprendi o ALIAS ( Muito Legal ) - Luis Quesada

git config --global alias.CAM 'commit -am' De forma global
git config alias.logpg 'log --pretty=oneline --graph' De forma local


Usando TAGs - Versões:

Registrando tag:
git tag -a [tag] -m [mensagem]
Vendo tags:
git tag

## Aula 7

O que foi que eu aprendi aqui?

Conectando repositorios - Luis Quesada

git remote add origin https://github.com/KaueMaia/AulaGIT.git

Enviando as atualizações para o repositório remoto:
git push origin master


Alterando no GitHub e recebendo no local:

Vamos no nosso repositório ver as alterações.
No próprio GitHub podemos fazer pequenas alterações e commits.
Baixar as atualizações do repositório remoto:
git pull origin master

Extra: Enviando tags para o repositório remoto:
git push origin master --tags


## Aula 8

O que foi que eu aprendi aqui?

aprendi organizar melhor meus projetos

Me organizar com Projects - Luis Quesada


## Aula 9

O que foi que eu aprendi aqui?

aprendi fazer um fork e trazer pro meu propio repositor

Graças a aula 9, consegui fazer um fork no seu repositório e solicitar algumas melhorias. Obrigado por tudo Kaue, voce é fera! - Luis Quesada
