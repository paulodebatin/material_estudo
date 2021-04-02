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
Exec=/home/paulo/ferramentas/eclipse/eclipse
Icon=system

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

-- ver número do ip local da máquina
hostname -I

-- vendo informações do processador
cat /proc/cpuinfo
lscp
lscpu | grep -E '^Thread|^Core|^Socket|^CPU\('

-- Telnet (testar conexão com um ip)
telnet
open
192.168.0.16 6379
