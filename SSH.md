# ssh config

## config 
1. generate key using ed25519
```
ssh-keygen -o -a 100 -t ed25519 -f ~/.ssh/id_ed25519 -C "perez.xochicale@gmail.com"
```

or rsa

```
ssh-keygen -m PEM -t rsa -b 4096 -C "perez.xochicale@gmail.com"
```


2. Adding your SSH key to the ssh-agent

```
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
ssh-add ~/.ssh/id_rsa
```


3. Adding a new SSH key to your GitHub account

sudo apt-get install xclip
xclip -sel clip < ~/.ssh/id_ed25519.pub
xclip -selection clipboard < ~/.ssh/id_rsa


New SSH and GPG keys
https://github.com/settings/keys


4. Testing your SSH connection

```
ssh -T git@github.com
Hi mxochicale! You've successfully authenticated, but GitHub does not provide shell access.
```


## refererences
* https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh
* https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
* https://help.github.com/en/github/authenticating-to-github/testing-your-ssh-connection
* https://medium.com/risan/upgrade-your-ssh-key-to-ed25519-c6e8d60d3c54
