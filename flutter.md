# Flutter

1) Instalar pacotes
flutter pub pub add <nome do pacote>

2) Atualizar os pacotes com base no pubspec.yaml
flutter pub get

3) Builder para produção
WEB: 
flutter build web 

APK: 
flutter build apk

4) Setar a sdk
flutter config --android-sdk="/home/paulo/Android/Sdk"

5) Ver versões
flutter doctor -v

6) Mudando para  versão 8 do java
export JAVA_HOME=/home/paulo/Downloads/android-studio/jre

7) Trabalhando com emuladores:
a) Vendo os emuladores: 
~/Android/Sdk/emulator$ : ./emulator -list-avds

b) Iniciando um 
~/Android/Sdk/emulator$ : ./emulator @Pixel_3a_API_30_x86

c) Rodar a aplicação com o emaulador
~/projetos/edusoft/pocs/frontend_flutter(feature/196422)$ : flutter run -d emulator 

8) Adicionando suporte da app para uma aplicação desktop (exemplo para Linux)
Na pasta do projeto:
> flutter create --platforms=linux .
Será criado o executável em ~projeto/build/linux/release/bundle
Para maiores detalhes: https://flutter.dev/desktop
