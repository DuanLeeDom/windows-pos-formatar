# Configuração Inicial do Windows

Se o computador já está formatado, siga as etapas abaixo para deixar otimizado o Windows:

## ETAPA 1: Ativação Windows e Office

1. Antes de tudo, faça uma verificação de atualização e se tiver, deixe atualizando normalmente no Windows, e se pedir para reiniciar faça a reinicialização e realize novamente e não deixe de baixar todas as atualizações por completo.

3. Abra o PowerShell em modo de `administrador` e execute o seguinte código:
   
    ```bash
    irm https://massgrave.dev/get | iex
    ```
4. Depois de executar o comando, siga as instruções abaixo:
   - [1] WHID | Windows | Permanent
   - Após a instalação, pressione Enter ou qualquer tecla.
   - [2] Ohook | Office | Permanent
   - [3] Dowload Office
   - Baixe a versão Microsoft 365 / Sub | Offline x86-x64 em: [Link para Download do Office](https://gravesoft.dev/download_windows_office/office_c2r_links/#portuguese-brazil-pt-br)
   - Baixe e instale o programa normalmente.
   - Após o download, volte às opções normais da tela Ohook Activation.
   - [1] Install Ohook Office Activation
   - Após a instalação, pressione Enter ou qualquer tecla.

## ETAPA 2: Antes de baixar qualquer coisa

Faça o download do recurso denominado `VisualCppRedist_AIO_x86_x64_82.zip`, extraia seu conteúdo e execute o programa conforme o habitual. É provável que o antivírus seja acionado, alegando que o programa é prejudicial, porém, isso não é verdadeiro, e você pode prosseguir com a execução sem preocupações.

1. Instale todos os Visual C++: [Visual C++ 2022 Redistributable](https://github.com/abbodi1406/vcredist/releases)

## ETAPA 3: App Installer Atualizar

1. Atualize o App Installer:

   ```bash
   winget update --all
   ```
   
   ```bash
   winget upgrade --all
   ```

2. Procurar um programa:

   ```bash
   winget search [nome do programa]
   ```

3. Instalar um programa:

   ```bash
   winget install [nome do programa]
   ```

# PROGRAMAS ESSENCIAIS

## PROGRAMAS
1. [AnyDesk](https://anydesk.com/pt) - Acesso Remoto

2. [RustDesk](https://rustdesk.com/) - Acesso Remoto Alternativo

3. [VLC](https://www.videolan.org/vlc/index.html) - Reprodutor Multimídia

4. [Audacity](https://www.audacityteam.org/) - Editor de Áudio

5. [OBS Studio](https://obsproject.com/) - Gravador e Transmissor de Vídeo

6. [FontBase](https://fontba.se/) - Gerenciador de Fontes

7. [DaVinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve/) - Editor de Vídeo Profissional

8. [Discord](https://discord.com/) - Plataforma de Comunicação para Gamers

9. [Google Chrome](https://www.google.com/intl/pt-BR/chrome/) - Navegador Web

10. [LibreWolf](https://librewolf-community.gitlab.io/) - Navegador Web Alternativo

11. [VirtualBox](https://www.virtualbox.org/) - Plataforma de Virtualização

12. [KeePassXC](https://keepassxc.org/) - Gerenciador de Senhas

13. [GIMP](https://www.gimp.org/) - Editor de Imagens

## JOGOS

1. [Steam](https://store.steampowered.com/about/) - Plataforma de Distribuição Digital

2. [Epic Games](https://www.epicgames.com/store/en-US/) - Loja de Jogos

3. [GOG GALAXY](https://www.gog.com/galaxy) - Loja de Jogos Sem DRM

4. [Ubisoft Connect](https://www.ubisoft.com/pt-br/game/ubisoft-connect) - Loja e Plataforma de Jogos da Ubisoft

5. [EA Origin](https://www.origin.com/) - Plataforma de Jogos da Electronic Arts

6. [Rockstar Games Launcher](https://www.rockstargames.com/rockstargameslauncher) - Plataforma de Jogos da Rockstar Games

# BAIXAR O WINRAR E TIRAR AQUELA PROPAGANDA

## Passos para Remover Anúncios do WinRAR

1. Baixar o WinRAR:
   - Faça o download do [WinRAR](https://www.win-rar.com/).

2. Criar o Arquivo de Registro:
   - Após o download, crie um novo arquivo de texto `.TXT` no seu computador.

3. Inserir os Dados de Registro:
   - Abra o arquivo de texto recém-criado e insira o seguinte texto:

     ```text
     RAR registration data
     SiM
     Local Site License
     UID=ca5575bd41c33ec5a2de
     6412212250a2de7c818d537f99bcf0218861216f4ce0738e2ef7ad
     8bc2514534357f5541ed60694c88f20734f7fa6ad968865654a57b
     0f0edf295d607ce6fa6d6b3667401b413bdcbccca3152c8ab6abc5
     931818a35674a26f065261f8bce32dfbce601d1aa079a3c54f79c7
     adeacb886214457e000e50d6ff5329a2f516ebba72708a35f704db
     3d30b1633de64c1bdc0c5c2b54710967dde4c9aab721b69460185e
     a12e2906a44bc32601e8ef0028d453a1d8b40dd23b562696892555
     ```

4. Salvar o Arquivo de Registro:
   - No menu do bloco de notas, selecione `Arquivo` e depois `Salvar Como`.
   - Navegue até o diretório onde o WinRAR está instalado normalmente em `C:\Program Files\WinRAR`.
   - Altere o tipo de arquivo para `Todos os Arquivos` para `(*.*)`.
   - Salve o arquivo com o nome: rarreg.key

Com isso, os anúncios não serão mais exibidos ao utilizar o WinRAR.

# Como Reparar o Windows com Apenas 3 Comandos

Executar o PowerShell como Administrador:

1. Comando:
   
   ```bash
   chkdsk /f
   ```
   - Este comando é capaz de encontrar e corrigir qualquer erro no disco rígido.

3. Comando:
   
   ```bash
   chkdsk /r
   ```
   - Esse comando é capaz de detectar e localizar os setores defeituosos no disco rígido de destino e tentar recuperar as informações legíveis dos setores defeituosos.

5. Comando:
   
   ```bash
   DISM /Online /Cleanup-image /Restorehealth
   ```
   - Esse comando é utilizado no Windows para verificar e corrigir a corrupção de arquivos de sistema. O DISM (Deployment Image Servicing and Management) é uma ferramenta de linha de comando que verifica a integridade da imagem do sistema operacional e tenta restaurá-la para um estado saudável. O parâmetro `/Cleanup-image /Restorehealth` especifica que o DISM deve tentar corrigir a imagem de sistema atualmente em uso.
