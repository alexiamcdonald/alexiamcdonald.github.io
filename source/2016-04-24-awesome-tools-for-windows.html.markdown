---
title: Awesome Tools for Windows
date: 2016-04-24
tags: example
---

#### Awesome Tools for Windows.

> “Asked about the fact that Apple's iTunes software for Windows
> computers was extremely popular, Jobs joked, 'It's like giving a glass of ice
> water to somebody in hell.” ― Walter Isaacson

#### Open the Windows.

When I first started University with the idea of being a programmer I had no
idea how easy I could make my life if I had just installed Linux. The computers
we were taught on pretty much all had Windows installed on them and only
some of the really serious people in my course had switched to Linux. I was
scared to the jump ship and knowing that my craptop had [hardware virtualisation](https://en.wikipedia.org/wiki/Hardware_virtualization) disabled it wouldn't be possible to switch back quickly if I
wanted to.   This is when I met [Brendan](https://github.com/bjz) who offered up his awesome
knowledge to me about the possibility of making Windows run a little bit like Linux.

!["Mmm chocolate"](http://i.giphy.com/cOWNPwDDh1tYs.gif)

#### Everything is better with Chocolate.

Windows, the land where open source software pages look like you are going to
download Malware.

> "Chocolatey is a package manager for Windows (like apt-get or yum
> but for Windows). It was designed to be a decentralized framework for quickly
> installing applications and tools that you need. It is built on the NuGet
> infrastructure currently using PowerShell as its focus for delivering packages
> from the distros to your door, err computer.

This is a must if you want to live the Windows life.  Install [chocolatey](https://chocolatey.org/) to free yourself!

#### Simba, Cmder...

Did you know you can have an awesome console on Windows? <blockquote>"Cmder
is a software package created out of pure frustration over the absence of nice
console emulators on Windows. It is based on amazing software, and spiced up
with the Monokai color scheme and a custom prompt layout. Looking sexy from the
start." </blockquote>  Well, welcome to the wonderful world of
[Cmder](http://cmder.net/). The place where no one knows how to pronouce
it and honestly we don't care because it's got multi tabs. YAY!  To
download this sweet terminal just go into what you currently have... either
Powershell or CMD and type in the following:  <kbd>choco install
cmder</kbd>  Pin it to your toolbar and you're good to go for the rest
of your Windows career.  *If it doesn't work you are probably missing* [Visual C++ Redistributable](https://www.microsoft.com/en-au/download/details.aspx?id=48145)

!["Simba dance"](http://i.giphy.com/szmmbDDpS67LO.gif)

#### Go crazy.

Now you are set to go and can download all the things! These two tools are
awesome and make life so much easier. There are heaps of awesome things you
could do.  You could install <b>Git:</b> <kbd>choco install git</kbd>
Or perhaps you want to run <b>Bash on Cmder:</b> <kbd>Open Cmder, then
click on the new tab menu, selecting the Setup tasks... option.</kbd>
<img src="../images/cmder-task-settings.png" alt="cmder setup"> Create a
new task by clicking the + button, and enter the following settings:
<b>Name:</b> <kbd>Git Bash</kbd> <b>Task parameters:</b> <kbd>/icon
"%ProgramFiles(x86)%\Git\etc\git.ico" /dir "%userprofile%"</kbd> <b>Commands:</b>
<kbd>""C:\Program Files (x86)\Git\bin\sh.exe" --login -i"</kbd>

Or maybe you want to code some <b>Ruby</b> <kbd>choco install ruby</kbd>
My personal favourite is to add my <b>SSH keys</b> <kbd>Open Git Bash
in cmder. Follow Github's <a
href="https://help.github.com/articles/generating-an-ssh-key/#platform-windows">instructions
for setting up your SSH keys</a> using ssh-keygen</kbd>  <i>The list goes
on...</i> Check all the packages on <a
href="https://chocolatey.org/packages">Chocolatey</a>  Have fun!

<a href="https://msdn.microsoft.com/en-au/commandline/wsl/about"><i>***This might soon be obsolete information as Windows has this plan where they make Linux work on Windows for realz***</i></a>


!["Welcome to the interwebs"](http://i.giphy.com/l41m1CuaT5Oy624Ra.gif)
