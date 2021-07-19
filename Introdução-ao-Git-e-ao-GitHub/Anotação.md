# Git #

Fucionamento do Git.
Tópicos;
1-SHA 1 = Algoritmo de encriptação (Identificadores de 40 dígitos).
	ex:
	echo "olá mundo" | openssl sha1
	> (stdin)= f9fc856e559b950175f2b7cd7dad61facbe58e7b
	ou
	opensslsha1 texto.txt
	SHA1(text0.txt)= f9fc856e559b950175f2b7cd7dad61facbe58e7b
	
BLOBS
TREES
COMMITS

Comandos básicos do git
-git init = inializa o repositório no git dentro da pasta
-git add
-git commit

*Crie um repositório (workspace/livro-receitas)
para primeiro acesso;
	terminal workspacw/livro-receitas
	$ git config --global user.email "email@email.com"
	$ git config --global user.name "usuário"
	

	$git add *
	$git commit -m "commit inicial" [ isso é a msg do commit] 
	$git push origin
	$git status

cire uma conta no github ou log.
crie um repositório

Terminal digite;
	$git remote add origin https:??
	$git remote -v : lista de repositório cadastrado
	$git push origin master

no caso de conflitos de versão de um arquivo já existente no github será necessário baixar a versão do github e fazer as alterações.(conflito)
	$ git pull origin master

para clonar um repositório do github.
	$git clone https://...
	
