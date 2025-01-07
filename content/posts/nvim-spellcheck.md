+++ 
draft = false
date = 2025-01-07T12:26:34+01:00
title = "Spell checking with Neovim"
tags = ["neovim", "nvim"]
categories = ["solutions"]
+++
Over the last years Neovim became my primary editor for almost everything. I edit a lot of markdown files, I obviously
need a spell-checker. I already new about including [LanguageTool](https://languagetool.org) through LSP, but found it
too much effort, since it relies on a local installation and I am already running LanguageTool in my local network.  
So, to no surprise I just learned that Neovim already comes with a basic spell-checker, which is good enough for my
purpose.

You can enable it with `:setlocal spell` and disable it again with `:setlocal nospell` - awesome.


