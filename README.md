# Learn-GitBranching
![https://learngitbranching.js.org/](https://www.scaler.com/topics/images/git-branching-strategy-thumbnail.webp)

[Click🥇learnGit-Branching!](https://learngitbranching.js.org/?locale=pt_BR)

# Compartilhar é se importar!


`Compartilhe árvores com seus amigos usando export treeeimport tree
Tem uma grande lição para compartilhar? Tente construir um nível com build levelou experimentar o nível de um amigo comimport level
Para ver todos os comandos, use show commands. Há algumas jóias como undoereset
Por hora, vamos começar com o levels...`
# Não compromete o Git
`Um commit em um repositório git registra uma fotografia (snapshot) de todos os arquivos em seu diretório. É como um grande copy&paste, mas ainda melhor!
O Git tem como objetivo manter os commits tão leves quanto possível, de forma que ele não copie cegamente o diretório completo toda vez que você fizer o commit. Ele pode (quando possível) compactar um commit como um conjunto de mudanças (ou um "delta" ) entre uma versão do seu repositório e a seguinte.`

`O Git também mantém um histórico de quando ocorreu cada commit. É por isso que a maioria dos commits tem ancestrais acima de si -- que indicamos usando setas em nossa visualização. 
Manter a história é ótimo para todos que trabalham no projeto! Há muito para aprender, mas por enquanto pense nos commits como snapshots do seu projeto. 
Os commits são muito leves, e mudar de um para outro é extremamente rápido!`

# Comandos Git

# Lista de Comandos:

# Comandos
## Iniciando um projeto #01
```
git init: Descrição : Comando para iniciar o repositório git. 
```
## Adicionando arquivos para commit #02
```
git add: Descrição : Comando para adicionar um ou mais arquivos em staging.
arquivo.txt: descrição : Nome de um ou mais arquivos.
```
## Como fazer um commit #03
```
git commit -m "alterações"

-m = flag para escrever uma mensagem de commit.
"alterações" = mensagem descrevendo ajustes.
OBS: Sem utilizar a flag -m: Acontece que um editor será aberto para digitar a mensagem commit.
```
## Conferindo os detalhes de um commit #04
```
git show: Descrição: comando que mostra detalhes de um commit.
exemplo adicionando 09c6d68: descrição: hash (identificador) do commit de interesse a ser analisado.
```
## Ambiente de staging #05
```
É a área de preparação dos commits, onde iremos ver a nossa coleção
de arquivos alterados ou criados que farão parte do próximo commit.
```
## Conferindo a lista de arquivos alterados #06
```
git status: Descrição: mostra o ambiente de staging.
```
## Conferindo o histórico #07
```
git log: Descrição: mostra uma lista interativa de commits
com o hash e a mensagem de cada commit.
```
## Adicionando arquivos para commit interativamente #08
```
git add: Descrição: Comando para adicionar um ou mais arquivos em staging = preparando os arquivos para envio.
-p: flag para escolher interativamente alterações específicas para commit.
```
## Criando um novo branch #09
```
git branch + [nome da branch a ser criada]: Descrição: Comando para criar uma nova branch, esse comando
apenas cria a branch, ainda é preciso trocar de branch para fazer commits.
```
## O que é um pull request #010
```
pull request: Descrição: É o processo de submeter alterações para revisão no GitHub.
No GitLab esse processo é chamado de merge request.
merge request:descrição: É o nome do mesmo processo do GitLab
```
## Mudando de branch #011
```
git checkout + [nome do branch de destino]: Descrição: Comando para mudar de branch e se deslocar para o destino.
```
## Conferindo as alterações de cada arquivo #012
```
git diff: Descrição: Lista de forma interativa as alterações de cada arquivo.
```
## O que é o HEAD #013
```
 HEAD: Descrição: É um ponteiro que indica em qual branch você está localizado.
É utilizado na hora de trocar de branches e de desfazer commits.
```
## Trocando de Branch ao criar um branch novo #014
```
git checkout -b [nome do novo branch]: Descrição: Comando para trocar de branch e ao mesmo tempo criar uma nova, com um novo nome.
-b: Descrição: flag para criar o branch.
```
## O que é um DIFF #015
```
diff:Descrição:Formato que representa alterações no projeto.
Adições:Descrição:São coloridas em verde e representadas pelo sinal de (+).
Remoções:Descrição:São coloridas em vermelho e representadas por um sinal de (-).

Formato que representa alterações no projeto.

Adições são coloridas em verde e representadas por um sinal de: (+).

Remoções são coloridas em vermelho e representadas por um sinal de: (-).
```
## O que é um FORK #016
```
O que é um Fork:Descrição:Nada mais é do que uma cópia de um repositório.
Essa cópia mantém um link com o repositório original.

Fork: Descrição:Nada mais é do que um cópia de um repositório.

Repositório original:Descrição:Essa cópia mantém um link com o repositório original.

Utilidade:Descrição:Comumente utilizado para propor alterações de código.
```
## O que é Clone #017
```
git clone [mais link do repositório]

O que seria o clone: Descrição: Fazer o clone ou clonar.
É a ação de baixar um repositório para o seu computador.

É possível clonar qualquer repositório desde que você tenha
acesso a ele.

Qual repositório você pode fazer o clone? É possível clonar qualquer
repositório desde que você tenha acesso a ele.
```
## Como fazer um clone #018
```
git clone [url]
Descrição:Comando para baixar o repositório + o url, caminho do repositório onde se encontra o mesmo.
```


