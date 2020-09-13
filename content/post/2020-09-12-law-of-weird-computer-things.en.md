---
title: Law of Weird Computer Commands
author: Christopher Gandrud
date: '2020-09-12'
slug: law-of-weird-computer-things
categories: []
tags:
  - symbols
  - computing
---

The QWERTY keyboard is one of the more commonly known examples of path dependence. It is the story of how a keyboard designed for a obsolete typewriter use case in the 1800s continues to influence the way we type.

Despite the persistence of the QWERTY keyboard letter layout, there was significant variation for all of the keys surrounding the letters until about the mid-1990s (when the current desktop operating systems--Windows, Mac, Linux--became dominant). This created a reverse-QWERTY. Keyboard layouts most people have never seen impact the programming languages and tools we use today. This leads to:

*The "Law" of Weird Computer Commands*:

> Any time a computer command seems weird, it's likely a path dependent consequence of keyboards not being standardised until the mid-1990s.

For example, Vim/Vi is the "[ubiquitous text editor](https://www.vim.org/)", especially for anyone working with Linux based servers. Just as ubiquitous, are the jokes about how difficult it is to [exit Vim](https://stackoverflow.com/questions/11828270/how-do-i-exit-the-vim-editor) (here is a [flow chart](https://stackoverflow.com/a/44201563)). You have to use the `ESC` key constantly, which is inconvenient for people with small hands on most keyboards these days. It was a real pain when Apple made the `ESC` a virtual button on the Touch Bar. The `h`, `j`, `k`, and `l` keys--all in one row on a QWERTY keyboard--are inexplicably used to move the cursor left, down, up, and right, respectively. 

These baffling command choices make sense once you see the [ADM-3A terminal](https://en.wikipedia.org/wiki/ADM-3A) keyboard used to develop Vi (source [Wikipedia](https://en.wikipedia.org/wiki/Vi#/media/File:KB_Terminal_ADM3A.svg)):

![ADM-3A keyboard layout](/post/2020-09-12-law-of-weird-computer-things.en_files/adm-3a-keyboard-wiki.png)

The `ESC` key is conveniently located not at the upper-left extremities of the keyboard, like you are probably used to, but more centrally where the `Caps Lock` key usually lives on modern keyboard. The `h`, `j`, `k`, and `l` keys served as the arrow keys, accessed with the `Ctrl`, e.g. `Ctrl+h` for left navigation.

[Apparently](https://en.wikipedia.org/wiki/ADM-3A#Legacy) the tilde `~` being located on the same key as `Home` inspired the use of `~` to denote the home directory in many Unix shells. 

Another strange computing thing that comes up in my work--primarily using computing for statistics--is that the assignment operator in the R language is `<-`. For example: `say_hello <- "Hello!"`. Many other languages (including R since the early 2000s) allow you to use `=` to assign values to objects. `=` is one fewer key stroke. What is the backward pointing arrow about? Chambers in [*Extending R*](https://www.amazon.com/Extending-Chapman-Hall-John-Chambers/dp/1498775713) notes that 

> The specific choice of `<-` dates back to the first version of S [which R is based on]. We chose it in order to emphasize that the left and right operands are entirely different: a target on the left and a computed value on the right. Later versions of S and R accept the `=` operator, but for exposition the original choice remains clearer.

Ok, doesn't seem to conform to The Law of Weird Computer Commands. But there is another layer to the story. Colin Fay [notes](https://colinfay.me/r-assignment/#:~:text=Historical%20reasons&text=This%20language%20used%20%3C%2D%20as%20an,had%20this%20sign%20for%20assignment.&text=So%20before%202001%2C%20the%20%3C%2D,assign%20value%20into%20a%20variable) that R is based on S, which was a bit inspired by [APL](https://en.wikipedia.org/wiki/APL_(programming_language)). APL use `←` for assignment. It had its own keyboard that actually included a `←` key. So at one time it would have been fewer key presses to use the dedicated backwards arrow key than the `=`, which was accessed with `Shift + 5`.
