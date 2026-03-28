**1. Herramientas necesarias**

```
sudo apt install -y git curl npm gcc ripgrep fd-find nodejs xclip
sudo apt install -g neovim
pip install neovim --break-system-packages
```

**2. Fuente JetBrainsMono**

```
mkdir -p ~/.local/share/fonts/JetBrainsMono
curl -LO --output-dir ~/.local/share/fonts/JetBrainsMono https://github.com/ryanoasis/nerd-fonts/releases/latest/download/JetBrainsMono.tar.xz
tar -xJf ~/.local/share/fonts/JetBrainsMono/JetBrainsMono.tar.xz -C ~/.local/share/fonts/JetBrainsMono
rm ~/.local/share/fonts/JetBrainsMono/JetBrainsMono.tar.xz
fc-cache -fv
```

```bash
Aplicar fuente en terminal:

Editar → Preferencias → Apariencia → Tipografía → JetBrainsMono Nerd Font Mono Regular
```

**3. Instalar Neovim**

```
sudo curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.tar.gz
sudo tar -C /opt -xzf nvim-linux-x86_64.tar.gz
sudo mv /opt/nvim-linux-x86_64 /opt/nvim
sudo ln -s /opt/nvim/bin/nvim /usr/local/bin/nvim
sudo rm nvim-linux-x86_64.tar.gz
```

**4. Instalar LazyVim**

```
git clone https://github.com/LazyVim/starter ~/.config/nvim
rm -rf ~/.config/nvim/.git
nvim
```

```
Verificar que todo está bien:

:checkhealth
```
