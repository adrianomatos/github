# RESUMO GIT E GITHUB 🐱‍👤
````
GIT CONFIG --GLOBAL USER.EMAIL "adrianotaua@hotmail.com"
GIT CONFIG --GLOBAL USER.NAME "Adriano"

GIT CLONE link_repositorio - Iniciar de repositório (clona rep web)
GIT CLONE link_repositorio novo_nome_pasta (se_quiser_mudar)
GIT CLONE link_repositorio --BRANCH FEATURE-1 --nome_branch_que_vc_quer

GIT INIT - Inicializa git na pasta atual
GIT BRANCH -M main (muda da branch MASTER para MAIN)
GIT ADD . - Adiciona tudo ou 
GIT ADD NOMEARQUIVO.EXT (add em staged antes de commit)

GIT COMMIT -M "msg de identificação do commit" (grava alterações locais)
GIT COMMIT --AMEND -M "renomeia msg do ultimo commit"
GIT COMMIT --AMEND (abre editor do vim, presiona i para editar msg de commit) esc :wq

GIT STATUS - Ver status de commits da pasta
GIT DIFF - Mostra as alterações em modified
GIT DIFF --staged - Mostra até alterações em staged
````

## CTRL+Z DO GIT 🙌
````
GIT LOG - Histórico de commits (autor, data, hash - Q p/ Sair)
GIT RESTORE nomeArquivo (desfazer alteração até último commit)
GIT RESTORE --staged nomeArquivo (desfazer alteração em staged/remove arquivo de STAGED)
GIT RESET nome_arquivo (remove arquivo de STAGED)
GIT RESET --SOFT hash_do_ultimo_commit (desfaz commit e deixa arquivos em staged)
GIT RESET hash_do_ultimo_commit 	(desfaz commit e deixa arquivos em untracked) ou
GIT RESET --MIXED hash_do_ultimo_commit (desfaz commit e deixa arquivos em untracked)
GIT RESET --HARD hash_do_commit_QUE_DESEJA (EXCLUI ARQUIVOS e COMMITS posteriores)
GIT REFLOG - mostra histórico de commits e alterações
````

## ENVIAR CÓDIGOS AO REPOSITÓRIO NO GITHUB (Rep. já criado) 🐱‍🏍
````
GIT REMOTE ADD ORIGIN https://github.com/adrianomatos/Blender.git
GIT REMOTE -V - Mostra repositórios cadastrados
GIT PUSH -U ORIGIN MAIN (MASTER <-> MAIN) Envia arquivos p/ GitHub (de MAIN p/ "Origin")
OU
GIT PUSH ORIGIN MASTER - Envia arquivos p/ GitHub (de Master [local] p/ "Origem" [na web])

GIT FETCH - Para baixar e ver alterações (p/ avaliar) antes de dar MERGE
GIR DIFF ORIGIN/MASTER (compara as 02 - Q p/ Sair)
GIT PULL - Para aceitar unir ORIGIN com MASTER (baixa e une alterações web c/ local))
GIT PULL ORIGIN MASTER - Trás as atualizações (s/ avaliar) ou git pull
````

## BRANCH - Desenvolvimentos paralelos em equipe ♻
````
GIT BRANCH - Lista branches
GIT BRANCH -a = listar todas as branchs do repositório remoto
GIT BRANCH nomebranchNova - Cria branch nova (com commit atual)
GIT LOG --ONLINE --DECORATE - Mostra commits RESUMIDOS e a branch atual 
GIT CHECKOUT nomebranchNova - Mudar para branch nomebranchNova 
... Alterações na nomebranchNova 
GIT CHECKOUT master - Para voltar para branch principal

UNIR (Merging) branches
GIT MERGE nomebranchNova (Une as 2 branches na branch master)
````

## ESTADOS DO GIT ⚠
````
UNTRACKED - NÃO MAPEADO/RASTREADOS
UNMODIFIED - Ñ MODIFICADO - MAPEADO
MODIFIED - EDITADO - TEM MUDANÇAS
STAGED - ADICIONADO AO GIT (PREPARADO PARA COMMIT)
````

## MARKDOWN E DICAS 😍
[Sintaxe básica de formatação do README](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
````
USAR VSCODE WEB PRESSIONANDO .
README.SO  - EDITOR DE README FÁCIL COM VISUALIZADOR
WINDOWS + . (MOSTRA MENU DE EMOJIS)
````

## PASTAS E ARQUIVOS 🤳
````
MKDIR NOME_PASTA
TOUCH NOME_ARQUI.EXTENSAO
ECHO NOME_PASTAouARQUIVO/ > .GITIGNORE
ECHO > .GITIGNORE (LIMPA GITIGNORE)
RM -RF .git (exclui pasta_repositorio_git)
