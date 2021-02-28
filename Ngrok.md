# Ngrok
O Ngrok expõe servidores locais atrás de NATs e firewalls para a Internet pública em túneis seguros.
https://ngrok.com/

1) Instalação:
a) Faça o download https://ngrok.com/download
b) Descompacte o arquivo: unzip /path/to/ngrok.zip	

2) Cria uma conta e faça a autenticação
a) Cadastro em: https://dashboard.ngrok.com/login
b) Gerando o token: Authentication (lado esquerdo do menu) > Your Authtoken
c) Autenticando localmente: ./ngrok authtoken <seu token gerado no item b>
Será gerado o arquivo ngrok.yml em disco. Em linux, geramente em /home/user. Ex: /home/paulo/.ngrok2/ngrok.yml

3) Expondo uma porta
./ngrok http 8080

4) Ajuda
./ngrok help



