# Criar um projeto
ng new <nome do projeto>
ng new app1-primeng

# iniciar a aplicação
ng serve

# mandando a aplicação para produção
ng build
    será criado uma pasta dist
    para testar, basta um http server (nginx, por exemplo) ou instale um como:
sudo npm install http-server -g
    depois é entrar na pasta dist e digitar:
http-server
    abra o browser e digite o path do index.html.    