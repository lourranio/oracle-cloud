# AMBIENTE 

## SUMARIO

- [VERSAO](#about)
- [UTORIAL EM VIDEO ](#video)


## About <a name = "about"></a>

Faca a instalação comando a comando.

Aqui o ambiente esta configurado com o ZSH + OH MY ZSH + FONTES.


## UBUNTU 20.04

```
    uname -a
```

## Installing

#!/bin/bash

### Executar comandos a seguir para atualizar os pacotes
```
    sudo apt update -y

    sudo apt upgrade -y

```

### Instalar pacotes a seguir
```

    sudo apt install dkms make perl gcc build-essential git curl -y
    
    sudo apt install build-essential zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev libssl-dev libreadline-dev libffi-dev libsqlite3-dev wget libbz2-dev

```


### Instalar Python 3.10 (opcional)

link: https://computingforgeeks.com/how-to-install-python-on-ubuntu-linux-system/

- 1 OPCAO

```
    sudo apt install software-properties-common -y

    sudo add-apt-repository ppa:deadsnakes/ppa

    sudo apt install python3.10 -y

    sudo apt install python3-pip -y

    python3.10 --version
```

- 2 OPCAO 

```
    sudo apt install python3.10-full python3.10-dev
```

## Baixar e instalar VS Code: https://code.visualstudio.com/download

## Baixar e instalar Google Chrome: https://www.google.com/intl/pt-BR/chrome/



# Instalar e configurar ZSH
```
    sudo apt install zsh -y
    
    chsh -s /bin/zsh
    
    zsh
```

# Instalar Oh-my-zsh! -> https://ohmyz.sh/
```
    sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

```

# Instalar Spaceship Prompt
# https://github.com/spaceship-prompt/spaceship-prompt

```
    git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1

    ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"

```

## Mudar ~/.zshrc -> ZSH_THEME="spaceship"

### Instalar Zsh Autosuggestions
### https://github.com/zsh-users/zsh-autosuggestions
```

    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

```
# Instalar Zsh Syntax Highlighting
# https://github.com/zsh-users/zsh-syntax-highlighting
```
    
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

```
## Mudar plugins ~/.zshrc 
```
    vim ~/.zshrc 
    plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

```

## Font optional (https://github.com/pdf/ubuntu-mono-powerline-ttf)
```
    mkdir -p ~/.fonts

    git clone https://github.com/pdf/ubuntu-mono-powerline-ttf.git ~/.fonts/ubuntu-mono-powerline-ttf

    fc-cache -vf

```

## TUTORIAL EM VIDEO <a name = "video"></a>
## VIDEO COMPLETO
https://www.youtube.com/watch?v=5i3TpDR8muU


</br>
</br>

### Para a plicar todas as configurações, reinicie a maquina/pc/notebook/desktop

### exec $SHELL que não precisa reiniciar. ou então dar um source .zshrc
