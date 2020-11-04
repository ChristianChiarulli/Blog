---
title: Java in Neovim
date: "2020-11-04"
image: "neovim.png"
author: "Chris"
tags: [Neovim_Java.png]
---

## Current State of Java + Neovim

**Available:**

- Treesitter highlighting
- Goto definition
- Goto references
- Formatting
- Diagnostics
- Hover
- Refactor/Rename
- Search files (FZF)
- Search text (FZF)
- Quickfix
- Lombok
- Configuration in `coc-config.json`

**Difficult to Implement:**

- Debugging

\* This can be done but in my opinion it's difficult to get setup, if you'd like to look further into it checkout the following:

- [nvim-dap](https://github.com/mfussenegger/nvim-dap)
- [vimspector](https://github.com/puremourning/vimspector)

### Note

You will need to have CoC installed I have a blog post and video for installing CoC here:

[YouTube Video](https://www.youtube.com/watch?v=OXEVhnY621M)

[Blog Post](https://www.chrisatmachine.com/Neovim/04-vim-coc/)

## Install

To realize most of the value make sure to install `coc-java`

```
:CocInstall coc-java
```

## Commands

Here are a bunch of commands to get the behavior of this video:

```
<Plug>(coc-codeaction)              " line action
<Plug>(coc-definition)              " definition
<Plug>(coc-references)              " references
<Plug>(coc-type-definition)         " type definition
<Plug>(coc-rename)                  " rename
<Plug>(coc-declaration)             " declaration
<Plug>(coc-implementation)          " implementation
<Plug>(coc-format)                  " format
<Plug>(coc-fix-current)             " quickfix
<Plug>(coc-codelens-action)         " code lens
<Plug>(coc-diagnostic-next)         " next diagnostic
<Plug>(coc-diagnostic-next-error)   " next error
:CocList diagnostics                " diagnostics
:CocList outline                    " search outline
:CocList -I symbols                 " references
:CocUpdate                          " update CoC
:CocDisable                         " disable CoC
:CocEnable                          " enable CoC
```

## Repo Links

[coc-java](https://github.com/neoclide/coc-java)