# Como instalar o Bpytop no Ubuntu 20.04 Linux via Snap

Passo 1. Abra um terminal;
Passo 2. Instale a versão estável do programa, usando esse comando:

```
  sudo snap install bpytop

```

Passo 3: Digite no terminal ``` bpytop ```



# Como instalar o Google Chrome no Ubuntu 20.04 via Repositório Oficial

```
wget -q -O - https://dl.google.com/linux/linux_signing_key.pub | sudo apt-key add -

sudo sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'

sudo apt-get update

sudo apt install google-chrome-stable

```


# Como instalar a última versão do VLC no Linux

```
  sudo apt-get install flatpak
  
  flatpak install --user https://flathub.org/repo/appstream/org.videolan.VLC.flatpakref
  
  flatpak --user update org.videolan.VLC
  
  sudo snap install vlc
