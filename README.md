obliviongit_example
===================

Exemplo de projeto no GitHub para aprendizado do projeto.

Git é uma ferramenta que auxilia no desenvolvimento de código aberto, assim como SVN e Mercurial. O git permite gerenciar problemas em arquivos em revisões diferentes, ou seja, mexer no arquivo tendo ele em dois estados ou mais e submeter apenas a revisão que deseja para o pai. Enfim, mesmo não tendo entendido, vamos entender ao longo do desenvolvimento do projeto de exemplo.

1. Fork(ando) em um projeto

Um fork de um projeto é apenas ter uma cópia do projeto pai. O fork é a sua cópia do projeto, você pode editar e submeter as modificações (chamado pull request), mas falaremos disso adiante. Para fazer um fork de um projeto no github basta abrir o projeto e apertar em fork. Você terá uma cópia do projeto em seu perfil.

2. Clonando o projeto para o seu computador

Para baixar o projeto do servidor para o computador é feito uma operação chamada clone. Ela pode ser executada com um comando:

git clone url.git <pasta_do_projeto>

parametros em <> são opcionais.

a url pode ser encontrada na página do projeto no github.

3. Commit/Pull/Push

Vamos agora entender como funcionam os comandos do git que podem ser listados e entendidos separadamente com um git --help.

O git é uma ferramenta que além de permitir programação colaborativa, permite também que um colaborador altere um arquivo enquanto outro colaborador altere a mesma parte do arquivo em periodos de tempo diferentes e mesmo assim resolva-se os conflitos de diferenças entre o código.

Vamos então entender como ele faz isso..

Quando você cria um arquivo pelo seu editor, ou por qualquer outro canto, você pode rodar um comando para verificar quais as mudanças feitas até agora e os arquivos que estão para ser adicionados (não rastreados), os rastreados e os deletados ou ignorados. Todos esses status podem serem obtidos com um comando:

git status

onde ? é não rastreado
A é adicionado
M é modificado
R é deletado
I é ignorado

caso todos os arquivos estejam não rastreados, use o comando:

git add .

onde . é o diretório atual, no caso pode ser substituido por qualquer arquivo ou pasta (caso seja uma pasta, todos os arquivos não rastreados daquela pasta serão adicionados)

Então temos um arquivo adicionado. A ideia de commit é uma mudança, problema, solução, qualquer coisa feita nos arquivos que termine uma parte de uma das coisas citadas acima é considerado um commit. Então se eu tenho um código que está dando erro de SQL e vou ajeitar, quando eu terminar de ajeitar, eu vou commitar os arquivos alterados. Um commit nada mais é do que colocar aqueles arquivos rastreados em stage para serem enviados para o repositório. ( como um elevador )
Um commit pode ser acompanhado de uma mensagem e é assinalado com suas credenciais, nome e email.

Para subir as mudanças commitadas para o repositório, se usa o comando:

git push

esse comando pelo github provavelmente pedirá seu usuário e senha do github.
E para receber os arquivos modificados de outras pessoas, poderá usar o comando:

git pull

Poderemos então criar cada um arquivo e subir para o servidor de vocês e enviar um pull request (na tela do projeto do github no seu fork do projeto) para mim.

4. Branches

Logo após explicarmos como funciona um gerenciador de tarefas, estilo redmine ou collabtive, explicarei sobre branches.
