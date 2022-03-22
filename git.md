# 1) Configuração Inicial do Git
$ git config --global user.name "Fulano de Tal"
$ git config --global user.email fulanodetal@exemplo.br

-- setando o editor padrão emacs
$ git config --global core.editor emacs 

-- listando as configurações:
$ git config --list

https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Configura%C3%A7%C3%A3o-Inicial-do-Git


# 2)  Fazer com que o git não solicite senha a cada push (GitHub)
$ sssh-keygen -- vai dando enter
$ cat ~/.ssh/id_rsa.pub

Acesse sua conta no GitHub, clique no canto superior direito na sua foto e depois em Settings (ou configurações).
Clique em SSH and GPG keys e depois em New SSH key.
Agora, você precisa colar a sua chave pública

# 3) Fazer com que o git não solicite senha a cada push (GitLab)
Acessa a conta do gitlab, sobre seu ícone de usuário, settings. Access tokens, dê um nome para o token, marque a opção api e clique em criar.
Com o token gerado, informe no link abaixo 

git remote set-url origin https://paulo.debatin:<token>@git.edusoft.com.br/mentorweb/edusoftapi.git

Exemplos:
git remote set-url origin http://paulo.debatin:Pi_jpv5Xk_rJRawMruwT@git.edusoft.inf.br/mentorweb/edusoftapi.git
git remote set-url origin http://paulo.debatin:Pi_jpv5Xk_rJRawMruwT@git.edusoft.inf.br/mentorweb/mentorweb.git
git remote set-url origin http://paulo.debatin:Pi_jpv5Xk_rJRawMruwT@git.edusoft.inf.br/mentorweb/edusoft-common.git

Se fizer a primeira vez o git clone conforme abaixo, não precisa fazer set-url:
git clone http://paulo.debatin:Pi_jpv5Xk_rJRawMruwT@git.edusoft.inf.br/mentorweb/edusoft-common.git

https://fullcycle.com.br/git-e-github/

# 4) How do you clone a Git repository into a specific folder?
git clone https://github.com/eugenp/tutorials.git  <nome da pasta>

# Adicionando uma pasta a um novo repositorio
echo "# flutter" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/paulodebatin/flutter.git
git push -u origin main

# Exemplo de como trabalhar com GitFlow
https://www.youtube.com/watch?v=wzxBR4pOTTs&list=PLDqnSpzNKDvkfF_ZMfukmOG3MtGKfXlfJ&index=5

# Mergeando uma branch para outra
Entrar na branch que irá receber as alterações e depois:
git merge feature/sua_branch
Mais informações: https://www.atlassian.com/br/git/tutorials/using-branches/git-merge
