# Guia Completo de Instalação do Flutter

Documentação de Instalação do Flutter no Windows para Desenvolvimento Mobile

Introdução

Esta documentação fornece os passos necessários para instalar o Flutter no sistema operacional Windows para desenvolvimento de aplicativos móveis (Android/iOS). O Flutter é um framework de UI open-source criado pelo Google para criar aplicações nativas de alta performance para mobile, web e desktop.

Pré-Requisitos

Antes de começar a instalação, assegure-se de ter os seguintes pré-requisitos:

- Sistema Operacional: Windows 7 ou superior (recomendado Windows 10 ou superior).
- Espaço em Disco: Pelo menos 1,64 GB de espaço livre em disco.
- Conexão à Internet: Acesso à internet para baixar os pacotes necessários.

Passo 1: Baixar o Flutter SDK

1. Acesse o site oficial do Flutter Flutter SDK (https://flutter.dev/docs/get-started/install/windows).
2. Baixe o arquivo ZIP para Windows.
3. Extraia o arquivo ZIP para uma pasta no seu computador, de preferência em um diretório fácil de acessar, como C:\src\flutter.

Observação:
Não extraia o Flutter em uma pasta com espaços no caminho (como C:\Program Files\Flutter), pois isso pode causar problemas ao executar o SDK.

Passo 2: Adicionar o Flutter ao PATH

Para garantir que você possa usar o Flutter de qualquer terminal, é necessário adicionar o Flutter ao PATH do sistema.

1. Abra o Menu Iniciar e procure por variáveis de ambiente.
2. Selecione Editar variáveis de ambiente do sistema.
3. No menu de Propriedades do Sistema, clique em Variáveis de Ambiente.
4. Na seção Variáveis de sistema, localize e selecione a variável Path e clique em Editar.
5. Clique em Novo e adicione o caminho para a pasta flutter/bin (Exemplo: C:\src\flutter\bin).
6. Clique em OK para salvar as mudanças.

Passo 3: Verificar a Instalação do Flutter

Agora, você precisa verificar se o Flutter foi instalado corretamente.

1. Abra o Prompt de Comando (ou PowerShell).
2. Execute o comando abaixo:

flutter doctor

O comando flutter doctor verifica seu ambiente de desenvolvimento e lista os requisitos que estão faltando ou precisam ser configurados. Caso haja alguma falha, o Flutter fornecerá instruções sobre como corrigir o problema.

Exemplo de saída esperada:

[√] Flutter (Channel stable, 3.3.5, on Microsoft Windows [Version 10.0.19043.1586], locale en-US)
    • Flutter version 3.3.5 at C:\src\flutter
    • Upstream repository https://github.com/flutter/flutter.git
    • Framework revision d21b1f5c83 (3 months ago), 2022-08-24 12:25:36 -0700
    • Engine revision 1dcd4b12ca
    • Dart version 2.18.3
    • DevTools version 2.12.2

[√] Android toolchain - develop for Android devices
    • Android SDK at C:\Users\SeuUsuario\AppData\Local\Android\sdk
    • Platform android-33, build-tools 33.0.0
    • ANDROID_HOME = C:\Users\SeuUsuario\AppData\Local\Android\sdk
    • Java binary at: C:\Program Files\Android\Android Studio\jre\bin\java
    • Java version OpenJDK Runtime Environment (build 11.0.11+8)
    • Android Studio at C:\Program Files\Android\Android Studio
    • Flutter plugin can be installed from:
      https://plugins.jetbrains.com/plugin/9212-flutter
    • Dart plugin can be installed from:
      https://plugins.jetbrains.com/plugin/6351-dart

[√] Chrome - develop for the web
    • Chrome at C:\Program Files\Google\Chrome\Application\chrome.exe

[√] Visual Studio - develop for Windows (Visual Studio not found)
    • Visual Studio not installed
    • Install Visual Studio to build Windows apps.
      Download at https://visualstudio.microsoft.com/

[√] Connected device (1 available)
    • Android SDK built for x86 (mobile) • emulator-5554 • android-x86 • Android 11 (API 30) (emulator)

• No issues found!

Se tudo estiver configurado corretamente, você verá uma mensagem indicando que o Flutter está pronto para ser usado.

Passo 4: Instalar Android Studio

O Android Studio é necessário para compilar e emular aplicativos Android.

1. Baixe o Android Studio (https://developer.android.com/studio).
2. Execute o instalador e siga as instruções.
3. Após a instalação, abra o Android Studio e configure o Android Virtual Device (AVD) para emulação de dispositivos Android.

Observação:
O Android Studio também pode instalar o Flutter e o Dart Plugin diretamente, caso você ainda não os tenha instalado.

Passo 5: Configurar o Emulador Android

Para testar seus aplicativos Flutter, você pode utilizar um emulador Android.

1. Abra o Android Studio.
2. Vá para Tools > AVD Manager.
3. Clique em Create Virtual Device.
4. Escolha o dispositivo desejado e siga as instruções para completar a criação do AVD.
5. Após a criação, inicie o emulador clicando no ícone de Play.

Passo 6: Criar seu Primeiro Projeto Flutter

Agora que tudo está configurado, você pode criar seu primeiro projeto Flutter.

1. Abra o Prompt de Comando ou PowerShell.
2. Navegue até o diretório onde você deseja criar o projeto.
3. Execute o comando abaixo para criar um novo projeto Flutter:

flutter create meu_app_flutter

4. Navegue até o diretório do seu projeto:

cd meu_app_flutter

5. Execute o aplicativo no emulador ou dispositivo conectado:

flutter run

Passo 7: Configurar o Visual Studio Code (Opcional)

Você pode configurar o Visual Studio Code (VS Code) como seu editor de código preferido.

1. Baixe o Visual Studio Code (https://code.visualstudio.com/).
2. Instale a extensão do Flutter e Dart:
   - Vá até Extensions no VS Code.
   - Procure por Flutter e Dart e clique em Install.
3. Após instalar as extensões, abra seu projeto Flutter no VS Code e você estará pronto para começar a desenvolver!

Conclusão

Com isso, o ambiente de desenvolvimento Flutter no seu Windows está pronto para o desenvolvimento de aplicativos móveis. Se você encontrar algum problema durante a instalação, consulte o comando flutter doctor e as sugestões fornecidas.

Para mais detalhes, consulte a documentação oficial do Flutter: Flutter Docs (https://flutter.dev/docs).

