### Initial Git Setup

Initial setting for Git

Source: https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup

#### Set users

``` shell
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

#### Set default branch name

``` shell
git config --global init.defaultBranch main
```

#### Set SSH

https://docs.github.com/en/enterprise-server@3.0/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account

https://www.youtube.com/watch?v=RGOj5yH7evk&t=1230s&ab_channel=freeCodeCamp.org


``` shell
ssh-keygen -t rsa -b 4096 -C "YOUR_EAMIL@example.com"


vim ~/.ssh/config 

Host *
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_rsa_personal


ssh-add -K ~/.ssh/id_rsa_personal

```
