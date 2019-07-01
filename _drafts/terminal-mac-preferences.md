---
layout: post
title: "Terminal macOS preferences"
---

oh-my-zsh

## Font

Dank Mono Regular 14 pt.

## Pure theme

### Install

```
npm install --global pure-prompt
```

### Edit 

```bash
code ~/.zshrc
```

Set `ZSH_THEME=""` in your `.zshrc` to disable oh-my-zsh themes.

### Add 

```
autoload -U promptinit; promptinit
prompt pure
```

[Repository](https://github.com/sindresorhus/pure)

## Syntax highlighting

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

```
plugins=(git zsh-syntax-highlighting)
```

[Repository](https://github.com/zsh-users/zsh-syntax-highlighting)