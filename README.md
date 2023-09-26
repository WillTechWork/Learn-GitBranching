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
git show: Descrição:
Comando que mostra detalhes de um commit.
Exemplo adicionando 09c6d68: descrição: hash (identificador) do commit de interesse a ser analisado.
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
git log: Descrição:
Mostra uma lista interativa de commits com o hash e a mensagem de cada commit.
```
## Adicionando arquivos para commit interativamente #08
```
git add: Descrição:
Comando para adicionar um ou mais arquivos em staging = preparando os arquivos para envio.
-p: flag para escolher interativamente alterações específicas para commit.
```
## Criando um novo branch #09
```
git branch + [nome da branch a ser criada]: Descrição:
Comando para criar uma nova branch, esse comando
apenas cria a branch, ainda é preciso trocar de branch para fazer commits.
```
## O que é um pull request #010
```
pull request: Descrição:
É o processo de submeter alterações para revisão no GitHub.
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
 HEAD: Descrição:
É um ponteiro que indica em qual branch você está localizado.
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

Descrição: Comando para baixar o repositório + o url, caminho do repositório onde se encontra o mesmo.
Exemplo: no terminal digite: git clone + o link do repositório + ENTER.
Após, dê o Open Folder ou Abrir a Pasta, localize o repositório.
E mão na massa para a criatividade do projeto! ;D
```
## O que é um REMOTE #019
```
É um repositório na nuvem por exemplo no github ou no gitlab.
Toda vez que você faz um clone, você tem pelo menos um remote -o origin.
remote: Descrição: É um repositório na nuvem por exemplo no github ou no GitLab.
informação extra: Toda vez que você faz um clone você tem pelo menos um remote - o origin.
```

## Como listar os REMOTES #020
```
git remote -v: Descrição: Comando para gerenciar remotes.

Sem usar o flag -v, você verá apenas o nome de cada remote.
Remote: Descrição: Comando para gerenciar remotes.

-v: Flag para mostrar detalhes do remote.
Informação extra:	Sem usar a flag -v, você verá apenas o nome de cada remote.

```
## Como criar um REMOTE #021
```
git remote add [nome do remote, a origem]

Descrição: Comando para gerenciar remotes e
           Comando para criar novos remotes.
           
```
## Como renomear um REMOTE #022
```
git remote rename atual novo

Descrição: Comando para gerenciar remotes.
           Comando para renomear o remote.
           Atual: Nome atual do remote.
           Novo: Novo nome do remote.
```
## Como criar o rastreamento do BRANCH no remote #023
```
git push --set-upstream remote branch

Descrição:

git push: comando para enviar alterações.
--set-upstream: flag para criar o rastreamento.
remote: repositório de destino.
branch: branch para fazer o acompanhamento.
```

## Como fazer o PUSH #024
```
git push remote branch

Descrição:

push: comando para enviar as alterações.
remote: repositório de destino.
branch: qual branch enviar.
```
## Apagando um BRANCH localmente #025
```
git branch -b [nome]
Descrição:

branch: comando para gerenciar branches.
-b: flag para apagar o branch localmente.
nome: nome do branch.
```
## Apagando um BRANCH forçadamente #026
```
git branch -D [nome da branch a que deseja apagar]
Descrição:

branch: Comando para gerenciar branches.
-D: CFlag para forçar a apagar o branch localmente.
nome: Nome do branch.
```
## Usando REBASE para atualizar um branch #027
```
git rebase origem destino
Descrição:

rebase: comando para reaplicar commits.
origem: branch mais atualizado.
destino: branch para atualizar, ou seja, que será selecionado para ser atualizado.
```
## Usando REBASE para corrigir a origem da branch #028
```
git rebase --onto origem anterior branch
Descrição:

rebase: comando para reaplicar commits.
--onto: flag para indicar a nova origem.
origem:  branch ou commit que deve ser a origem.
anterior: origem incorreta do branch.
branch: branch que precisa da correção.
```
## Como remover um arquivo de STAGING #029
```
git restore --staged [nome]
Descrição:

restore: comando para restaurar o estado anterior.
--staged: flag para olhar arquivos em staging.
nome: nome do arquivo.
```
## O que é um conflito #030
```
Acontece quando duas ou mais alterações são realizadas
no mesmo pedaço de um arquivo e o git não sabe como aplicar a
alteração mais recente.

Conflitos: São indicados pelos marcadores.
>>>, ===, e, <<<
conflito:descrição: Comando para fazer o download do repositório.
```

## Ajustar o último COMMIT #031
```
git commit --amend

commit: descrição: comando para lidar com commits.
amend: descrição: flag para corrigir o último commit.

Obs: Por padrão o amend fará o ajuste do último
commit gerando um novo commit.
```

## Descartando ALTERAÇÔES #032
```
git restore [nome]

restore:descrição:comando para restaurar o estado anterior.
[nome]:descrição:nome do arquivo.
Obs: As alterações descartadas não estão em staging.
```

## Fazendo um CLONE nomeado #033
```
git clone [url nome]

git clone:descrição: comando para fazer o download do repositório.
url:descrição: caminho do repositório.
nome:descrição: nome da pasta de destino.
```
## Mudando de BRANCH #034
```
git switch [nome]

nome: descrição: nome do branch.
switch: descrição: comando para troca de branch.
```
## Mudando de BRANCH ao criar um branch novo #035
```
git switch -c nome

switch:descrição: comando para troca de branch.
-c:descrição: flag para criar novo branch.
nome:descrição: nome do branch.

```
## Desfazendo COMMITS recentes #036
```
git reset HEAD ~3

reset:descrição:comando para restaurar um estado anterior.
HEAD:descrição: ponteiro que indica o estado atual.
~3:descrição: quantidade de commits a serem desfeitos.
```

## Desfazendo o último COMMIT #037
```
git reset HEAD^

reset:descrição: comando para restaurar um estado anterior.
HEAD:descrição: ponteiro que indica o estado atual.
^:descrição: o circunflexo é um atalho para o último commit.
```
## Desfazendo COMMITS de forma soft #038
```
git reset HEAD^ --soft

reset:descrição: comando para restaurar um estado anterior.
HEAD:descrição: ponteiro que indica o estado atual.
^:descrição: o circunflexo é um atalho para o último commit.
--soft:descrição: flag para guardar alterações em staging.
```
## Reaproveitando COMMIT #039
```
git commit -c ORIG_HEAD

commit:descrição: comando para lidar com commits.
-c:descrição: flag para reaproveitar a mensagem de commit.
ORIG_HEAD:descrição: cópia do estado anterior contendo a mensagem do commit anterior.
Obs: Se precisar editar a mensagem, use a flag -c.
```
## O que é STASH #040
```
stash:descrição: É um conjunto de alterações que ficam salvas em uma pilha.

utilidade:descrição: O comando permite salvar as mudanças feitas e voltar para um
estado limpo, ou seja, sem mudanças, do seu diretório de trabalho.

"n" em stash@{n} indice do stash
```
## Fazendo o STASH de mudanças #041
```
git stash push

stash:descrição: comando para gerenciar stashes.
push:descrição: comando para criar um novo stash.
Obs: o push pode ser omitido.
```
## Nomeando um STASH #042
```
git stash -m "alterações"

stash:descrição: comando para gerenciar stashes.
-m:descrição:flag para escrever uma mensagem de stash.
entre os "":descrição: mensagem para descrever às atualizações propostas, ou seja, escrevendo a descrição da alteração.
```


