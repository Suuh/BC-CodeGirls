# Comandos no GIT

echo "seu texto" | exibir um texto
openssl sha1 NomeDoArquivo | para gerar/exibir o sha1 daquele arquivo
cd | navega até a pasta
cd .. | volta uma pasta
ls | lista os arquivos da pasta atual

git init | inicializa reporitorio
git status | Informa os status de tudo e dos arquivos não editados ou editados mas não comitados
git add | adiciona o arquivo no stage para ser comitado
git commit -m "texto informativo das mudanças" | comita as alterações e manda junto um texto breve resumindo o que aquele commit altera/faz
git remote -v | para mostrar quais repositórios remotos o commit está linkado
echo > nome-do-arquivo.txt | criar arquivo no modo untrack
git add * | move o arquivo criado de untrack para staged

como criar uma branch da main:
git checkout nome-da-branch-que-quer-acessar | para se mover pelas branch desejadas
git checkout -b nova-funcionalidade | para se mover pelas branch e criar nova branch chamada nova-funcionalidade

como juntar branchs:
você se move até a branch que vc quer, e dentro dela você pede para fazer a fusão da branch que deseja juntar com ela.
ex: juntar na barnch main e branch nova-funcionalidade:
git checkout main  | para se mover para a branch main
git merge nova-funcionalidade | para juntar as duas

para mudar o nome de uma branch estando dentro dela:
git branch -m novo-nome

para mudar o nome de uma branch estando dentro de outra branch:
git branch -m nome-da-branch-que-quer-mudar novo-nome
ex: git branch -m funcionalidade nova-funcionalidade

para deletar branch:
git branch -d nome-da-branch-que-quer-deletar

para criar um stash:
Stash serve para guardar os arquivos de uma branch que estão no modo staged, e não levá-los par outra branch quando se movimentar. Funciona como uma array.
git stash save "msg explicando oq está fazendo"

para ver os arquivos que estão no stash:
git stash list

para pegar um arquvio em específico do stash para utilizá-lo ou commitá-lo etc:
git stash pop 1 | aqui no caso o nº 1 é o índice(posição) do arquvivo dentro do stash 

para limpar o stash:
git stash clear






como mudar de master para main:

