# 1) Configuração Inicial do Git
$ git config --global user.name "Fulano de Tal"
$ git config --global user.email fulanodetal@exemplo.br

-- setando o editor padrão emacs
$ git config --global core.editor emacs 

-- listando as configurações:
$ git config --list

https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Configura%C3%A7%C3%A3o-Inicial-do-Git



# 2)  Fazer com que o git não solicite senha a cada push
$ sssh-keygen -- vai dando enter
$ cat ~/.ssh/id_rsa.pub

Acesse sua conta no GitHub, clique no canto superior direito na sua foto e depois em Settings (ou configurações).
Clique em SSH and GPG keys e depois em New SSH key.
Agora, você precisa colar a sua chave pública

https://fullcycle.com.br/git-e-github/


