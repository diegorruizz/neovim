#### Herramientas necesarias

```
sudo apt install -y gcc default-jdk python3 python3-pip python3-venv git curl xclip npm nodejs ripgrep fd-find lazygit fzf
sudo npm install -g neovim
pip install neovim --break-system-packages
```

#### Fuente JetBrainsMono

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

#### Neovim

```
sudo curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.tar.gz
sudo tar -C /opt -xzf nvim-linux-x86_64.tar.gz
sudo mv /opt/nvim-linux-x86_64 /opt/nvim
sudo ln -s /opt/nvim/bin/nvim /usr/local/bin/nvim
sudo rm nvim-linux-x86_64.tar.gz
```

#### LazyVim

```
git clone https://github.com/LazyVim/starter ~/.config/nvim
rm -rf ~/.config/nvim/.git
nvim
```

#### Autocompletado

```
Ejecuta :Mason

Selecciona (2) LSP pulsando 2
```

- Python
    
    Busca `pyright` y pulsa `i` para instalarlo.
    
- C
    
    Busca `clangd` y pulsa `i` para instalarlo.
    
- Java
    
    Busca `jdtls` y pulsa `i` para instalarlo.
