#Comandos Linux

-- ver tamanho dos arquivos-
ls -lah

-- apagar um diretorio
rm -rf diretorio

-- copiar todos os arquivos de um diretório para outro
cp -a /home/paulo/ferramentas/eclipse/. /snap/eclipse


-- criar um atalho
- touch  /usr/share/applications/eclipse.desktop
- chmod +x /usr/share/applications/eclipse.desktop
- nano /usr/share/applications/eclipse.desktop
[Desktop Entry]
Name=Eclipse
Type=Application
Exec=/home/paulo/ferramentas/desenvolvimento/start.sh
Icon=/home/paulo/ferramentas/desenvolvimento/eclipse/icon.xpm


-- adicionar/atualizar variável de ambiente
export JAVA_HOME=/home/...

-- ver variáveis de ambiente
printenv

-- ver apenas uma variável
echo $JAVA_HOME

-- Compactação. Exemplo compactando a pasta Projetos:
tar -czf projetos.tar.gz Projetos/
A primera coisa que você deve ter notado é que, diferente do zip, o comando tar não necessita do -r. Ele age de forma recursiva por padrão. O -c é de create, ou seja, para indicar que desejamos criar um arquivo. O -z indica que queremos compactar com gzip. Utilizamos o -f (file), para que o comando crie o arquivo compactado.

-- Descompactação
tar -xzf projetos.tar.gz

-- Procurar arquivos
find / -iname pagamentos.*

-- Ver diretório atual:
pwd

-- criar um diretorio
mkdir nome_pasta

-- apagar diretório
rm -rf <nome>

-- ver número do ip local da máquina
hostname -I

-- vendo informações do processador
cat /proc/cpuinfo
lscp
lscpu | grep -E '^Thread|^Core|^Socket|^CPU\('


https://elias.praciano.com/2015/09/comandos-para-obter-informacoes-do-seu-sistema-ubuntu/


Outras formas:
htop
gotop man

-- Telnet (testar conexão com um ip)
telnet
open
192.168.0.16 6379

-- Mudar o prompt de comando
PS1=" »»» "

-- Ver processos para poder matá-los
Pressione as teclas ALT + F2 e digite: gnome-system-monitor e dê enter

-- minimizar a jabela aberta ao clicar no ícone
> gsettings set org.gnome.shell.extensions.dash-to-dock click-action 'minimize'

-- TMUX
> sudo apt install tmux
> tmux
Dividir painel na vertical: CTRL+B,	%
Dividir painel na horizontal: CTRL+B, “
Navegar entre os paineis CTRL+B, setas
Eliminar o painel: CTRL+B, x
Listas as sessoes: tmux ls
Restaurar uma sessão fechada: tmux attach-session -t <indice da janela>
Matar definitivamente a session: tmux kill-session -t <indice da janela>


- Atalhos Linux
Colaca a janela para direira: Super + seta para direita 
Colaca a janela para esquerda: Super + seta para esquerda
Maximiza  a janela: Super + seta para cima
Minimiza  a janela: Super + seta para baixo
Abrir terminal: CTRL+ALT+T

-- Ver portas em uso
lsof -i -n
netstat -nlp | grep :8081
-> Para matar o processo:  kill -9 <id processo>

-- Forma boa para listar arquivos
ls -lha

-- Personalizar linha de comando
sudo apt install zsh
https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh
Para escolher os temas: https://github.com/ohmyzsh/ohmyzsh/wiki/Themes
cd ~
sudo nano .zshrc
