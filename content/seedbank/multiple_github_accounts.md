---
title: GitHub Multiple Accounts in One Device
tags: ["github", "pwsh", "dev", "seed", "note"]
---

Reference - [fromDev2Dev](https://www.youtube.com/watch?v=Fyfp0oEWD6w&ab_channel=fromDev2Dev)

### Enable Service

Go to ==services.msc== and enable **OpenSSH Authentication Agent**; Set the Startup as 'Automatic'

### Create Private and Public Keys for Account

>[!info] repeat for all user accounts

```bash
ssh-keygen -t ed25519 -C "test@domain.com"
# provide filename, example id_25519_test
# provide password
```

>[!tip] by default, location of keys will be ~/.ssh, if not found, check under current directory and move the files under ~/.ssh


>[!note] file without extension is private key and with .pub extension is public key

### Add Keys in Github

>[!info] repeat for all user accounts

Go to github account and from settings, go to ==SSH and GPG keys== and add the public key with custom *title*, set *key type* as Authentication Key


###  Create SSH config file

Create ==config== file under ~/.ssh using the following format

```bash
Host github.test // hostname can be customized
    Hostname github.com
    User git
    IdentityFile ~/.ssh/id_25519_test
    IdentitiesOnly yes
    
```
