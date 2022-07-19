# Conceitos importantes do GIT
### SHA1:
SHA1 (Secure Hash Algorithm) é um algoritmo de incriptação. Possui um conjunto único de identificação com 40 dígitos de caracteres. É uma "chave de identificação" que representa um arquivo em específico.

### Objetos Fundamentais:
#### BLOBS:
As famosas Bolhas do Git que armazenam arquivos que possuem metadados. A Blob um objeto que possui: Tipo; Tamanho; \0; Conteúdo do arquivo (que pode ser txt, binário, etc). Ela guarda o sha1 daquele arquivo. 

#### TREES:
As árvores do Git. Elas armazenam/apontam para as Blobs. Elas possuem os metadados: Tipo; Tamanho; \0; e a Blob para qual ela aponta e também exibe o arquivo daquela blob. Ela tbm possui um Sha1 único dela. (sha1 daquela tree.
A Tree é a responsável por montar toda a estrutura de onde estão localizados os arquivos. Elas podem apontar tanto para Blobs como para outras Trees.

#### COMMITS:
Objeto que junto tudo!
Um Commit aponta para uma Tree;
Um Commit aponta para um Parente (Parente é o último Commit realizado antes dele);
Um Commit aponta para um Autor (a pessoa responsável, que fez o commit);
Um Commit aponta para uma Mensagem (que explica o que aquele commit faz);
Um Commit possui um Timestamp (Tempo, data/hr que foi criado);
Um Commit possui Tamanho;
Um Commit possui um SHA1 próprio dele;

#### CHAVES SSH E TOKENS