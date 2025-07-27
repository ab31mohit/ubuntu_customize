# ubuntu_customize
This guide helps to customize your Ubuntu Desktop to give it a new lool. 

## Install dependencies :   

```bash
sudo apt  update
sudo apt install git
sudo apt install curl
```

## Customiziing terminal with starship : 

1. Install starship

   ```bash
   curl -sS https://starship.rs/install.sh | sh
   ```
   Source starship

   ```bash
   echo 'eval "$(starship init bash)"' >> ~/.bashrc
   ```
   [Official doc is here](https://starship.rs/).

2. Change default Gnome Terminal theme to Dracula

   ```bash
   sudo apt-get install dconf-cli
   ```

   ```bash
   git clone https://github.com/dracula/gnome-terminal
   cd gnome-terminal
   ./install.sh
   ```
   [Official doc is here](https://draculatheme.com/gnome-terminal).

## Cutomizing Gedit theme to Dracula : 

  ```bash
  wget https://raw.githubusercontent.com/dracula/gedit/master/dracula.xml
  ```
  ```bash
  mkdir -p .local/share/gedit/styles/
  mv dracula.xml $HOME/.local/share/gedit/styles/
  ```
  Now open Gedit and select Dracula theme from preferences.     
  [Official doc is here](https://draculatheme.com/gedit).

