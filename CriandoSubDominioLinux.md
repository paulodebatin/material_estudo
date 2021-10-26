#Criando subdomínio no Linux

Ex.: saas.sistema.com.br apontar para localhost

a) instalar nscddaemon.
sudo apt-get install nscd

b) liberar cache
sudo service nscd restart

c) Editar arquivo de host
nano /etc/hosts

127.0.0.1 saas.sistema.com.br

d) Para acessar o sistema
http://saas.sistema.com.br


http://saas.sistema.com.br:8082/api/actuator/prometheus
http://ace.mentorweb:8082/api/actuator/prometheus
http://modular.mentorweb:8082/api/actuator/prometheus

curl -i --header 'kong-debug: 1' http://ace.mentorweb:8000/cal/api/actuator/prometheus