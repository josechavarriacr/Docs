---
slug: install-config-nvm
title: Install & Config NVM
authors: [josechavarriacr]
tags: [nvm, nodejs, npm]
---
Install and config Node.js with NVM  
Note: the next config works only in Bash and <span style={{color: "red"}}>does not work in fishshell.</span>



<!-- truncate -->

Install NVM via Homebrew:

```bash
brew install nvm
```

Then, create a directory for nvm:

```bash
mkdir ~/.nvm
```

Add the following lines to your shell profile (~/.zshrc):

```bash
export NVM_DIR=~/.nvm
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This load$
```

Restart your terminal, or source the profile file:

```bash
source ~/.zshrc 
```

List installed versions:

```bash
nvm ls
```

List available versions:

```bash
nvm ls-remote
```

Install a specific version (e.g., version 16):

```bash
nvm install 16
```

Switch Between Node.js Versions:

```bash
nvm use 16
```

Set a default version:

```bash
nvm alias default 16
```
