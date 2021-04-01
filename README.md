# clippit-for-webdirect

An implementation of [clippy.js](https://github.com/smore-inc/clippy.js) for FileMaker WebDirect

<p align="center"><img src="https://get.stephancasas.com/static/clippit-for-webdirect.png" width="85%"></p>
<p align="center"><i>Clippit, harrassing users inside of my <a href="https://github.com/stephancasas/webdirect-font-utility">webdirect-font-utility</a> demo file.</i></p>

---

## What is this?

Clippit (yes, that's right, **Clippit**, not *"cLiPpY"* — see the [Wikipedia article](https://en.wikipedia.org/wiki/Office_Assistant)) was once a staple *(no he wasn't — he's clearly a paperclip)* in the Microsoft Office suite of applications.

Based on the now-infamous Microsoft Agent API, Clippit would eventually find his way to being the most-hated anthropomorphized paper fastener in all of modern history. Despite offering useful advice, and shipping with an *Animate!* function that became a source of deep procrastination for teenagers and office workers with quickly-approaching deadlines, Clippit was removed from all versions of Microsoft Office after Office 2007.

With **clippit-for-webdirect**, you can diminish the value of the robust UI you've built for your FileMaker databases  running on the sleek FileMaker WebDirect platform, by adding Clippit right into the mix!

## Is this real?

Yes.

## Why?

Why not?

## Install

Setting-up clippit-for-webdirect is easy! Just follow these simple steps:

1. In your existing FileMaker solution, create a new web viewer on your entry layout.
2. In the web viewer's URL, paste the contents of [`clippit.fmcalc`](https://github.com/stephancasas/clippit-for-webdirect/blob/main/clippit.fmcalc).
3. Check the option for *Automatically encode URL*
4. Shrink, or visually hide (don't use the *"hide object when"* option) the web viewer, and hit *Save*!
5. I don't know what comes after this, but it probably isn't good.

## Customize

Want to make the most out of this awful experience? Of course you do. Why else are you still reading?

You can customize clippit-for-webdirect by making changes to the content of [`clippit.fmcalc`](https://github.com/stephancasas/clippit-for-webdirect/blob/main/clippit.fmcalc):

### Messages

To change what Clippit says, add your own messages under the `CLIPPIT MESSAGES` comment, like this:

```plaintext
/*--- CLIPPIT MESSAGES ---*/
"Let's delete this record for fun!";
```

You can also change the rate at which Clippit interrupts your users. Edit the value under `MESSAGE INTERVAL`.

### Animate Interval

Want Clippit to do tricks? Hell, yeah! Set the value under the `ANIMATE INTERVAL` comment to anything other than `0`.

### Boring Stuff

If you don't trust my server or jQuery's server, you can host your own copies of jQuery and `clippit.min.js`. Upload to wherever you'd like, and then change the values under `STYLESHEET & JS`.

## A Note From the Developer

I should've been writing invoices instead of working on this.

## License

Is this even worth licensing? MIT, or whatever, yeah...