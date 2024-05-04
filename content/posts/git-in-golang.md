---
title: "Git in Golang"
date: 2024-04-26T11:12:15+03:00
draft: false
---

## Nice excercise

Recently I stumbled upon [codecrafters](https://codecrafters.io/), a wonderful resource for learning programming. So I decided to try their course called 'Build your own Git'. In the best traditions, I skipped the last stage, because it is a bit scary. I would probably revisit it some time later. Other than that, I implemented the basic commands of working with blobs, trees and commits. And I think that was quite pleasent experience. It is not a complicated excercise, and it's marking as 'medium' seems fair. Of course there were some troubles here and there. Important points that I had discovered during that time were as follows:

 - If you are using something that needs to be closed, watch it carefully. Don't forget about deferred close calls. But remember that sometimes you have to close manually in order to flush buffer data.

 - Always look for others code to see how other people approach the same problem. This may give you an inspiration, offer a different angle, and familiarize you with wider subset of the language.

 - If you have a gut feeling that you are doing it wrong, then most probably that you are indeed. Think about how you could approach your problem from different angle and try to seek information about it. 

 - If some abstractions exist out there, like writer, reader or buffer, there probably is a good reason for it. Look closely at what these abstractions are, and what do they offer. You may find it surprisingly useful.

Difficulty of this excercise and scale with complexity of each stage feel the exact size of what you would need. After some poking around and familiarizing with basic libraries and concepts, coding begins. It is not too easy to be boring, and not too hard to be frustrating. Besides, it offers a good learning experience and perspective. Unfortunately, I could not use customly writed automated tests, but I could implement it nevertheless. Ultimately, I probably would recommend this type of challenge.
