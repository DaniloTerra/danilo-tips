# Workflow
- Criar repositório
- Criar, editar, excluir arquivos ao Working Directory
- Adicionar ou Remover arquivo ao Staging Area
- Salvar alterações do Stage ao Repository

# Básico

## Criar um repositório GIT
- git init

## Visualizar o status do Working Directory e Stage
- git status

## Adicionar arquivos do Working Director ao Stage
- git add nomeDoArquivo

## Comparar um arquivo do Working Directory ao Stage
- git diff nomeDoArquivo

## Confirmar as alterações do Stage ao Repository
- git commit -m "mensagem do commit"

## Visualizar os históricos de commits
- git log


# Branchs

## Listar branchs
- git branch
- git branch -a, --all (lista os remotos)

## Criar um branch no GIT
- git branch nomeDoBranch

## Mudar de branch no GIT
- git checkout nomeDoBranch

## Fazer merge
- git checkout nomeDoBranchEstável
- git merge nomeDoBranchModificado

## Excluir branch no GIT (local)
- git branch -d nomeDoBranchASerExcluido

## Excluir branch no GIT (remoto)
- git push origin --delete nomeDoBranchASerExcluido
