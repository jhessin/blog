---
title: "Apple - Love to Hate or Hate to Love?"
date: 2021-10-16T09:52:53-06:00
draft: false
---

# Apple - My Love Hate relationship with it

I have been an apple fan ever since a friend of mine introduced me to the
platform in high school. I have always liked their design concepts and the feel
of their OS. As soon as I could afford it I went out and bought an iMac, then
an iBook, then a MacBook Pro. The reliability of their OS and the high quality
of their hardware has always been a key selling point - along with the
uniformity of their platform.

That being said there have been several times that I have been frustrated with
the design choices that Apple has made. I remember the first time was shortly
after I bought my first iMac and they announced that they were moving away from
the PowerPC architecture and would be building new macs with Intel chips. One
of their selling points at the time (for me at least) was the use of the RISC
architecture and I had just gotten the iMac with a PowerPC chip. So all the new
software needed Intel while I had a PowerPC.

Quickly on the heels of this decision was the advent of OS X. My iMac had OS 9
on it and I was just getting used to that. I'm not going to say OS X was a bad
decision on their part (I LOVE OS X), but at the time it was quite the
adjustment.

Over time as the world has gone more and more toward cloud-based computing
Apple has taken a larger and larger share of the market. They went from a niche
to mainstream - no one baulks at finding out you own a Mac anymore. It's gotten
to the point that there isn't even a windows machine in my house.

I often joked that Apple takes good ideas and perfects them. That's what they
did with the smartphone (iPhone), and wearables (Apple Watch).

# Development - The other side of the coin

## Enter the Rabbit Hole!

On the other side I have found the development road with apple a painstaking
one. The standardization is great - I know what language I should be using to
develop software, and what tools I should utilize. On the other hand these same
standards feel stifling when compared to the wide world of computing. There are
several technologies that I have become enamored with.

## Rust - Systems programming for the next generation

First there is Rust - the programming language. I really enjoy writing and
troubleshooting it. It is refreshing to have a systems programming language
that has so much type safety to keep a programmer from falling in a rabbit
hole.

Rust seems to work great with Apple architecture - but the problem comes when
trying to display any kind of GUI - there are no hooks for rust to access
Apple's GUI systems. The only way to really accomplish it is by writing a
system library that then is called by Swift code. But if I wanted to write in
Swift I would write in Swift - not Rust. Another option is to use GTK or
another Linux library that will work with OS X - but the look and feel of those
applications are definitely lacking.

You may say - why not stick with Swift - it's a good language. You'd be right,
but the issue is that Swift only really works with Apple. Cross-Platform is
not good with it. Rust is a "System Level" programming language. This means
that it should be able to be written at the system level and not care about
the OS it is run on.

## Progressive Web Apps - Cross Platform for everyone?

So what system should I use for a GUI that works across all platforms?
Progressive Web Apps seem to check all the boxes. The issue I have had with
these is they are only installable on desktops as chrome apps for offline use.
On my iPhone I need an internet connection every time I launch the app no
matter what. I think Android may have the same issue - but I don't have a
device to test it.

Another issue is that these are invariably written using JavaScript and HTML.
These technologies have been around forever and, while they have improved
greatly, they still bear the scars of old bugs. The type safety in JavaScript
is non-existent, and Typescript is only a pittance toward the goal. I have used
many libraries such as Next.JS and Stencil/Ionic to name a few. Stencil seems
to use Typescript to great effect, but it is still JavaScript behind the
scenes.

## Enter Flutter/Dart - The future of web development?

I just recently discovered Flutter/Dart and its growing ecosystem of modules.
It has much stronger type safety and hosts a great deal of tools for building
both Progressive Web Apps and native applications for multiple platforms. I
found writing dart code strangely reminiscent of Rust - mainly because of the
"Sound Null Safety" that it ensures.

All that said debugging can be tricky. There is no console access in Flutter -
and there are a lot of bugs in published flutter/dart packages. I have gotten
pretty far in a project just to find that the tool I'm trying to use is broken
and I need to find another. I have never had this issue with Rust code.

# Okay - out of the rabbit hole!

Sorry for getting side tracked there. I was talking about Apple. The latest
thing that they have done is leaving Intel in the dust once again. The M1 chip
is all the rage right now - supposedly much faster than Intel, but now running
other OS's is a non-starter.

The more I think about it the more I think Apple is simply stubborn. Take the
charging cable they use for the iPhone for example. They have been using the
same lightning cable forever - I always thought it was superior because it can
be plugged in either direction unlike the old mini/micro USB cords. Then USB-C
came around and offers the same benefit for Android devices. Does Apple jump on
the bandwagon and start using the same cord? No - they keep pushing the
lightning cord. Now they have released a new iPad that takes a USB-C charger,
but they still insist the lightning cord is better.

Display ports are the same - the mini-ports that my PowerBook sports are so
fickle that I can barely keep an external monitor working - but they insist
they are better than the mini-HDMI that other systems use, though I haven't had
any issues with them.

# Conclusion?

I don't think there is one. To develop Apple software (especially iPhone
software) an Apple computer is a must. But I find Linux a much better
supported and easier to handle OS. I like the stability and standardization of
the iOS but miss the customization and diversity of Linux that Android sports.
I like the look and feel of Mac OS (especially the fonts), but I really love
the extreme level of customization that Linux supports.

I think the main deciding factor that I have is about the mobile OSes. Android
is always proprietary - and has zero standards. This means if you buy an
Android phone you will always get a different system that looks and feels just
a touch different than your last. That is why I have always stuck with iPhone.
That by extension is why I have stuck with Mac - because I need a Mac to
develop for iPhone.

The solution would be to develop a fully customizable Android that pulls the
users preferred look and feel from the cloud so they can keep the same
experience regardless of phone - nix the proprietary customization because it
is NOT a selling point. Unfortunately I don't know how this would be done.
