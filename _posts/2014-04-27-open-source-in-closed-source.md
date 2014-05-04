---
layout: post
title: "Open Source in Closed Source"
description: ""
category: "Engineering"
tags: ["open source", "closed source", "free software",
"responsible disclosure"]
---
{% include JB/setup %}

A lot of products in the Silicon Valley are built by plumbing together open
source software modules, self-developed proprietary modules and the underlying
framework using a proprietary layer. The open source modules are more often than
not an essential piece of the puzzle, (re)developing them would lengthen
development time significantly. However, it is often unclear how proprietary
software can use open or free software while honoring its license. A lot of
times you can ignore the problem, for example if you are running a website or
providing some other kind of service. If we are honest, it's more an ethical or
moral problem, because nobody will ever find out anyways. However, if you ship
something to the costumer, for example a library or an application, it gets
trickier, because others can take a look and see what you are doing. And they
will, for example
[Busybox](http://www.busybox.net/) and [FFMPEG](http://ffmpeg.org/) even
maintained halls of shame in
[the](http://web.archive.org/web/20100216045911/http://busybox.net/shame.html)
[past](http://web.archive.org/web/20101214233906/http://ffmpeg.org/shame.html).
The rule of thumb fall-back that I use personally is to avoid
[GPL](https://www.gnu.org/licenses/licenses.html) and credit all
[Apache](http://www.apache.org/licenses/LICENSE-2.0.html) or
[BSD](http://opensource.org/licenses/BSD-2-Clause) licensed usage.

Being an [open source contributor](https://github.com/FabianFrank) myself, I
think it is great if you use code that I wrote and I personally prefer licenses
that allow myself and others to reuse open source in the easiest way possible.
However, acknowledging the usage of open source is important to me, especially
if the author of the code required it in their license.

What triggered me into writing this post is an issue that I came across
recently when looking at different library offerings that solve a certain
mobile development problem. Some of them closed, others open source. There were
fully open and fully closed offerings available. Upon taking a look at the
closed offering I found what I expected, a product that looked like what I
described in the opening paragraph and sadly they don't acknowledge any Open
Source Software Software usage, despite the
[Apache 2 License](http://www.apache.org/licenses/LICENSE-2.0.html) and
[New BSD License](http://opensource.org/licenses/BSD-3-Clause) requiring
them to do so. If you look at the libraries that they use, it's very obvious
how to plumb them together yourself to achieve the desired result and there are
even open source projects doing it for you.

Now I have been thinking for quite a while if and how I should call them out.
Finally today I came to the conclusion to send them an E-Mail and give them a
chance to rectify their hopefully honest mistake. Mainly because I believe you
should never blame people for mistakes, but only for not wanting to learn from
them. Of course also because I'd appreciate a heads up if you ever find an
embarrassing mistake that I made or could at least fix. Let's see if
[responsible disclosure](http://en.wikipedia.org/wiki/Responsible_disclosure)
works for open source licensing violations. As a community we easily
acknowledge the general importance of Open Source Software Software, but often
fail to admit how big its part is in our own most recent proprietary works.

What would have you done if you were in my position? What would you do if the
violating company doesn't respond or will state that they won't fix the problem?
Let me know your thoughts in the comments.

<b>Update:</b> The company has responded to me and told me they will address the
issue in their next sprint. I'm excited to see what happens.
