
# Removendo arquivos grandes do histórico do Git

## Baixe o BFG
link: `https://rtyley.github.io/bfg-repo-cleaner/#examples`

## Clonar o repositório do Git
Pode clonar o repositório via código ou pelo Gir Desktop
`git clone https://empresa@dev.azure.com/Power%20BI/_git/Projeto_01`

## Remove files larger than 20M
Onde `C:\teste\bfg-1.14.0.jar` é o caminho do programa e `C:\Repos\Projeto_01` é o caminho do repositório clonado do Git

`java -jar C:\teste\bfg-1.14.0.jar --strip-blobs-bigger-than 20M C:\Repos\Projeto_01`

## Limpar os Arquivos
`git reflog expire --expire=now --all && git gc --prune=now --aggressive`
