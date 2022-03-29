# Install and setup zsh

**Backup bashrc**

```bash
cp ~/.bashrc ~/.bashrc_bak
```

**Install zsh**

```
{
  sudo apt update
  sudo apt install zsh -y
}
```

Change the shell by running:

```bash
chsh
```

Now add this path `/bin/zsh`, now log out and in for the changes to take effect.

At next terminal start choose 0 to configure empty `.zshrc`.

**Install oh-my-zsh**

Run

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

**Zsh autosuggestions**

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

Now add the plugin to the list of plugins in `.zshrc`:

```bash
plugins=( 
    # other plugins...
    zsh-autosuggestions
)
```

Restart the terminal or `source .zshrc`.


**Zsh syntax highlighting**

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```


Now add the plugin to the list of plugins in `.zshrc`:

```bash
plugins=( 
    # other plugins...
    zsh-syntax-highlighting
)
```

**Fonts**

```bash
sudo apt install fonts-font-awesome
```
