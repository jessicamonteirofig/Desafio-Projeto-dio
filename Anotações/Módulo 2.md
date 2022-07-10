# Introdução ao Git e ao GitHub

Olá. Este é o espaço onde transcreverei todas as minhas anotações sobre a matéria "Introdução ao Git e ao GitHub". Por ser uma disciplina mais prática não há tantas anotações assim, porém, tentarei transmitir tudo que eu absorvi durante as aulas. Eu utilizo o windows e minhas anotações estão baseadas nos comandos para o windows. Minhas notas de aula estão divididas por tópicos e são eles:

- O que é Git ?
- Comandos básicos para navegar no terminal
- Entendendo como o Git funciona
- Primeiros comandos com o Git
- Ciclo de vida dos arquivos
- Trabalhando com o GitHub
- Resolvendo conflitos

Antes de começar a listar minhas anotações, irei disponibilizar aqui o link para a instalação do Git:

https://git-scm.com/ 

Link da página do Git que possui documentação, manual e vídeos explicativos:

https://git-scm.com/doc

Espero que gostem!

### O que é Git?

Git é um sistema de versionamento de código distribuído. Foi criado por Linus Torvalds (criador do Linux). 

### Comandos básicos para navegar no terminal

Para abrir o terminal do Git basta pesquisar na barra de tarefas "Git bash". O Git bash já será quando você instalar o Git. Caso você queira abrir o Git bash dentro de uma pasta específica basta clicar com o botão direito do mouse e selecionar a opção "git bash here".

- Para listar pastas ou para saber onde está, basta digitar: dir (windows) e ls (linux e mac) e em seguida apertar enter.
- Para navegar entre as pastas basta digitar: cd "nome da pasta que quer entrar" /, e em seguida apertar enter.
- Para sair de uma pasta: cd ..
- Limpar a tela: clear ou cls
- Criar uma pasta: mkdir "nome da pasta que deseja criar"
- Criar arquivos dentro de uma pasta: echo > "nome do arquivo que deseja criar"
- Deletar arquivos: del
- Deletar repositórios: rmdir "nome da pasta" /S /Q

## Entendendo como o Git funciona

SHA 1 

-> Secure Hash Algorithm (Algoritmo de Hash seguro)

-> É um conjunto de funções hash criptográficas projetadas pela Agência de segurança nacional dos EUA. A encriptação gera um conjunto de caracteres identificador de 40 digitos.

-> Uma particularidade dele é que se for gerado um sha1 para um arquivo de texto e depois esse arquivo de texto for modificado em apenas uma vírgula, o sha1 desse arquivo modificado será diferente.

-> Abrir sha1 de um arquivo:  openssl sha1 "arquivo"

### Objetos internos do Git

- **Blobs**: Armazena arquivos, contém metadados e possui sha1.
- **Tree**: Tem metadados, aponta para um blob ou para outra árvore, armazena blobs, monta estrutura de onde estão os arquivos, tem sha1.
- **Commit**: Aponta para uma árvore, um parente, um autor e uma mensagem, possui timestamp, possui sha1.

### Chaves SSH e Tokens

É necessário utilizar uma dessas formas de autenticação para poder empurrar seus códigos para o GitHub de maneira segura.

**Chave SSH**: É uma forma de estabelecer uma conexão segura e encriptada entre duas máquinas.

​	Como criar: no próprio terminal basta escrever: ssh - keygen -t ed25519 -c "seu email", dessa 	maneira serão geradas duas chaves, uma pública e uma privada e é isso que vai garantir a segurança. Depois é necessário acessar o conteúdo dessa chave pública e informá-la ao github, para isso basta digitar o comando: cat id_ed25519.pub no terminal e é só copiar o número da chave e colar no local apropriado na página do GitHub. 

A segunda parte consiste em criar a conexão com um ambiente de desenvolvimento local (a sua maquina), pois o servidor (github) irá reconhecer e não será necessário fazer login sempre que você quiser empurrar um código. Dessa maneira, utiliza-se o mesmo comando para  mostrar a chave privada: cat id_25519, e então é só copiar e informar ao terminal com o comando: eval $ (ssh -agent -s) "chave privada".

**Token de acesso pessoal**: Para gerar o token basta ir na página do github, acessar developer settings -> personal access token -> generate meu token e então é só copiar e salvar em um local seguro.

## Primeiros comandos com o git 

### Criando um repositório

- Para inicializar um repositório basta digitar "git init" no  terminal

- Para mostrar arquivos ocultos digite: flag ls -a

- Para configurar seu nome e email basta digitar um de cada vez: git config --global user.name (para o nome ) e git config --global user.email (para o email)

- Para alterar essas configurações de nome e e-mail desfazer e depois refazer:

  ​	git commit --global --usent user.name, e depois: git commit --global user.name

  ​	o mesmo serve para o e-mail.

### Ciclo de vida dos arquivos 

![](C:\Users\waldi\OneDrive\Imagens\image-1.webp)

- Tracked: são arquivos que o git já conhecem e podem ser classificados em unmodified, modified e staged.
- Untracked: são arquivos que o git ainda não conhece.

* O ciclo se repete toda vez que um arquivo é alterado.

- O comando "git add .arquivo" transforma um arquivo de untracked para staged
- git status mostra o status dos arquivos e se tem algo que precisa ser commitado
- para commitar um arquivo basta dar um git add * para passa-lo para staged e entao um git commit -m "arquivo" (sugiro dar um git status para conferir que tudo foi commitado).
- se após o commit for criado outro arquivo ou pasta, ou até mesmo modificados, o git mostrará como "untracked" e será necessário realizar o commit novamente
- Para mover um arquivo para dentro de uma pasta basta digitar: mv "nome arquivo" ./ "nome pasta" /
- Para adicionar um arquivo como index: git commit -m "adiciona index arquivo"

- Para passar o repositório local para o repositório remoto: git remote add origin "link do repositório remoto" e depois é só empurrar para o repositório remoto com o comando: git push origin master (esse master também é comum aparecer como main, é só olhar como está cadastrado na sua máquina)
- Para mostrar repositórios remotos cadastrados: git remote -v

### Resolvendo conflitos

##### Conflito de merge: 

Ocorre quando altera-se um arquivo depois de empurrar para o github e tenta-se commitar e empurrar novamente. O git não irá aceitar a alteração. Contudo, para reparar esse erro é bem simples, basta puxar o que já foi feito com o comando: git pull origin master. Em seguida é só realizar as alterações que você deseja, realizar o commit e então empurrar novamente ao github.
