---
title: "Build Toolchain and Scripting"
date: 2024-04-23T11:44:12+03:00
draft: false # Set 'false' to publish
tableOfContents: false # Enable/disable Table of Contents
description: ''
categories:
  - Build Toolchain
  - Scripting
tags:
  -
---

## Systems organization and tooling

Recently I am reorganizing my DSA folder, where I keep my primitive data structures and algorithms implementations in C. Since C is quite old language, it has its own problems when it comes to such tasks as compiling and file organization. For example, setting up a compiler is no easy task. It is not as simple and lightweight as something like Python or Go. There are a lot of compilers, and many of them are pretty heavy or somewhat troublesome. I think, that people on Linux don't suffer from these problems, because everything that could be needed for them is included in `build-essentials`. On Windows, on the other hand, it is not so nice and simple as one package. The most optimal solution here probably is to use Microsoft C++ compiler included in Visual Studio. I am not a huge fun of VS, but they seems to provide building tools, which includes everything that you need without IDE. Exactly what I needed. 

After some poking around, I became curious about how to use those tools. Of course, I could just use VSCode, since everything needed is configured almost automatically here. As I mentioned earlier, I don't really like those huge and heavy IDEs with GUIs which take eons to download, install and launch. CLI tools are generally faster and more flexible. So I started to poke around. Apparently, CLI version supports almost anything that you could possibly need. But it requires from you to read documentation. Also, there are pretty much all tools that you could need: assembler, linker, etc. But unfortunately one piece is missing here: debugger. Debugger is not included in build tools, but you can get it either from Windows SDK, or as a standalone tool. One other problem is a build manager. Apparently, you can use makefiles with nmake tool. Altough it is possible to use it, but it doesn't provide much flexibility, and uses rather obscure syntax. 

One thing that I don't like about windows is that there is some sort of dualism in scripting world between cmd and powershell. Cmd is kinda annoying because it uses its own commands like dir or del instead of ls or rm, which is slightly pissing me of. And old scripting tools have quite tedious syntax. And generally it is just annoying that there are too many tools to use many of which are either binded to a specific platform or require some actions to obtain: Bash Shell, Windows CMD, PowerShell... It is just keeps going on. And there are some languages available like Python or Lua. Another problem for me is that with WSL you essentially obtain a new operating system with its own tooling. So, now there is no virtual machine or multiboot, but still there are two systems, each of which requires its own maintenance.

That kind of dualism is frustrating in some sense. Eventually, what we have is two worlds: Windows and Linux. And while Windows is absolutely dominant on the PC market, and virtually everyone is using it, Linux is still much more comfortable environment for the developers, because it has a very sweet tooling almost out of the box, like bash, git, gcc, gdb, etc. And even if something is missing, you can fix it by typing `sudo apt install x`, and it's done. It's worth notice though, that situation is definetly improving: now windows have a lot of tools like powershell, winget or wsl, which make life easier.
