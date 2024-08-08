Setup WSL2 on windows

```
wsl --install
```

Update packages
```
sudo apt update && sudo apt upgrade
```

Install brew
```
test -d ~/.linuxbrew && eval "$(~/.linuxbrew/bin/brew shellenv)"
test -d /home/linuxbrew/.linuxbrew && eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
test -r ~/.bash_profile && echo "eval \"\$($(brew --prefix)/bin/brew shellenv)\"" >> ~/.bash_profile
echo "eval \"\$($(brew --prefix)/bin/brew shellenv)\"" >> ~/.profile

sudo apt-get install build-essential procps curl file git
```

Setup Git
```
git config --global user.name "Your Name"
git config --global user.email "youremail@domain.com"

brew install gh
gh auth login
```

VSCode WSL
```
code .
```

Add brew to .bashrc path if needed.
