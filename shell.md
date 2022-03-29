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


