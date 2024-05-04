---
title: "Blockchain in Golang"
date: 2024-04-21T07:48:21+03:00
draft: false # Set 'false' to publish
tableOfContents: false # Enable/disable Table of Contents
description: ''
categories:
  - Blockchain
  - Golang
tags:
  -
---

## Reflection on complexity

Despite of how much time already passed since I started to learn how to code, it certainly doesn't feels like I am steadily improving that much. Nevertheless, it is still quite fun to try some things now and then. Recently I discovered such wonderful resource as [build your own x](https://github.com/codecrafters-io/build-your-own-x). Essentially, this is kind of collection of tutorials on how to build some stuff. Although they certainly vary on topics and complexity, there are some worthy ones. After some beginner stuff, like cli tools and chat bots, time came to do some serious business. More precisely, I decided to give a shot for [blockchain tutorial in golang](https://jeiwan.net/posts/building-blockchain-in-go-part-1/), since it sounded intriguing. Well, I am somewhat grateful to that tutorial in the sense that it make more clear some points that had not been that clear for me before.

 - Complexity is a function of quantity. The more code you have, the more difficult it is to remember all of the stuff. It is important to navigate 'on the fly', and look for information on the spot, infering your solution step by step
 - It is important to have a clear vision. It is hard to refactor code all of the time. Your changes can break things easily, so it is good if you can plan some things ahead to save yourself from some pain. Bad solutions can stick to your code pretty easily due to the cost of refactoring
 - Your code has to be flexible enough. Often it is not possible to implement everything you want at once. As you start from the core skeleton, features are gradually added to your code. For that reason, it is important to be able to adjust for those changes. You can think about it as a good part of the design.
 - And finally. Code is akin to mathematical equations from world of quantative descriptions of the world. It is rigorously precise and carry very clear and defined meaning, but at the same time it was designed for humans to understand. Although it is often the case that it is really difficult to infer meaning of the code from the first glance, it is still definetly possible. Code is bad for describing general and abstract ideas and principles behind its actions. Instead, it describes them way too precisely. And from that description it is then possible to infere abstract ideas.

Back to the blockchain. First three parts were fairly easy. I think this is the scope that is covered in most of the blockchain tutorials. That was quite fun and enlightening, since the concept of the blockchain is really simple. It is just a chain of blocks which is bonded together by hashing. It is all that there is to it. But of course, it is not enough to implement, say, cryptocurrency. At that point, some really scary and nasty stuff begins. Transactions, inputs, outputs, wallets, public key encryption... There is way too many stuff behind way too many black boxes. It is quite tricky to somewhat get it. But nevertheless, I probably can say that now I have some sort of vague idea behind it. Last part, on networking is really scary, so it had been left unimplemented.  
