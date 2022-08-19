**🐧 LINUX**
------------

### 🔺 Instalação Git

🔸 **1.** Abra o terminal (Ctrl + Alt + t) e vamos verificar se temos o git instalado:

    git --version

🔸 **2.** Execute o comando:

    sudo apt-get install git-all

🔸**3.** Confirme novamente se o git realmente está instalado:

    git --version

🔸 **4.** Vamos começar as configurações iniciais:

**4.1** Cofigurar o nome de usuário

    git config --global user.name "Seu nome"

​ **4.2** Configurar o endereço de e-mail:​ _É de suma importância que o ENDEREÇO DE E-MAIL SEJA O MESMO DO GITHUB afim de evitar conflitos!_

    git config --global user.email seuemail@email.br

 **4.3** Vamos conferir a lista de configurações:

    git config --list

🔸 **5.** Pronto, git instalado e configurado com sucesso!

**🪟 WINDOWS**
--------------

### 🔺 Instalação Git

🔹**1.** Entre no site ofical do [**GIT**](https://git-scm.com/downloads)

🔹**2.** Escolha a opção Windows e o instalador será baixado automáticamente

🔹**3.** Mantenha as opções pré selecionadas e siga com Next

🔹**4.** Install

🔹**5.** Antes de finaizar a instalação, selecione a opção Lauch Git Bash

🔹**6.** Ao finalizar o passo 5, irá abrir o Git Bash

🔹**7.** Agora vamos fazer as configurações iniciais:

🔹**8.** Confirme se o git realmente está instalado:

    git --version

🔹**9.** Vamos começar as configurações iniciais:

​ **9.1** Configurar o nome de usuário

    git config --global user.name "Seu nome"

​ **9.2** Configurar o endereço de e-mail:​ _É de suma importância que o ENDEREÇO DE E-MAIL SEJA O MESMO DO GITHUB afim de evitar conflitos!_

    git config --global user.email seuemail@email.br

​ **9.3** Vamos conferir a lista de configurações:

    git config --list

🔹**10.** Pronto, git instalado e configurado com sucesso!

## :wrench: Configurando chave SSH

🔹**1.** Acesse sua conta do [**GIT**](https://git-scm.com/)

🔹**2.** Clique no seu perfil na área superior direita e depois em **Settings**

🔹**3.** No canto esquerdo, procure por **SSH and GPG keys**

🔹**4.** Abra o **Git Bash** já instalado  e digite o código abaixo:

    ssh-keygen -t ed25519 "seu e-mail"

🔹**5.** Vai pedir autenticação, então digite a senha que irá gerar duas chaves SSH, uma privada e uma pública (*.pub*)

🔹**6.** Navege até a pasta .ssh criada e liste as chaves criadas por meio do comando *ls*

🔹**7.** No **git bash** digite e copie a chave que gerar

    cat id_ed25519.pub

🔹**8.** No site do GitHub, em **SSH and GPG keys**, clique em *New SSH Key* e cole a chave gerada. Dê um nome para a máquina

🔹**9.** De volta no **git bash**, hora de startar a chave

    $ eval $(ssh-agent -s)

    ssh-add id_ed25519

🔹**10.** Seu GitHub foi linkado com sua máquina!
