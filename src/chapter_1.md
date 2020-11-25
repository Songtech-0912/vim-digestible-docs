# Quick Start 

First off, I should highlight that Vim is my personal preference, not because of its endless configuration or its minimalist charm, but by its permissive and open license. 

My personal point of view is that large companies such as Microsoft and Adobe <ul>will inevitably use free and open-source as a marketting gesture</ul>, not a genuine commitement. But take a look at the Vim community, and you'll basically be staring at Github repos all day. Vim is truly the epitome of decentralization (ok, with maybe emacs just beating it by a margin). Its plugin system and overall architecture simply exuberates community, even if "free and open-source" isn't even on the frontpage of its website.

## What to do if you struggle with vim

I understand the frustration you can get when first using vim. I felt the same way when I tried to learn vim and gave up twice. Vim just felt so unneccesary - why `:q!` if you can use CTRL Q in every other program? Why `:w` when you've always used CTRL S? And my least favorite command: `ggVG"+y` to copy the document. Every little quirk of vim can spiral onto a full-blown case of Vim frustration.

So how do you avoid the classic syndrome of "Vim depression"? I've generally relied on several ways to do so:

### Use the GUI versions first

The Vim community has ardently resisted against a GUI for Vim for decades. That's why most versions of Vim are pretty minimal, out of the box. It has to be launched from a command line. Copy and paste doesn't work. And click-drag select does nothing - which can utterly break people.

That's why I recommend installing a GUI version of Vim. For Windows and GNU/Linux, it usually means GVim. For Mac users, MacVim should also do a good job. I might recommend neovim GUIs such as Veonim and Goneovim, but these are not ready-to-download and must be compiled.  

Let's get back on topic here. If you open up GVim or MacVim, the user interface is, to put bluntly, not spectacular. Yes, you can highlight, copy, and paste, and yes, you can move the cursor with a mouse, but it just doesn't look right. Which is why you need to beautify Vim.

### Make Vim colorful

Right out of the box, Vim is practical drawing pad, not a polished work of art. However, Vim was never designed to be a plain drawing pad with no drawings on it. Vim was always intended to look how you wanted it to - and it can look pretty good - even better than many modern editors - once you begin adding themes and plugins.

First things first, the most visually altering things you'll need to do are:

- Install a new theme
- Install an airline status bar
- Install coding fonts 

Installing a font is probably the first and easiest one of the three. And so on...

### Focus on the navigation

Vim's 4-key based navigation is arguably its strongest point. That's how it never needs to rely on a mouse to work.

However, getting to grips with this can be difficult. And even worse are keyboard tables for Vim, which, though well-intentioned, provide little true support.

So that's why learning visually is a great idea. Take this, for example:

```
	k
	^
	|
   h <-- --> l
	|
	v
	j
```

This is a good way to get familiar with Vim's 4 key navigation. And once you're done with that, try this:

```
   <-|------------------------------|->
     0     |   <-<- |  ->->   |     $
       <---+        *     <---+--->
       b          here    w       e
               ^ <-<-
```

After that, it's just a few sparse commands that muscle memory will eventually get the hang of, such as `gg` to go to the top of the document, `number G` to go to a specific line, and `G` to go to the last line. Work in progress...



Now, with SPC e, I can launch a file browser (coc-explorer), make a `index.html` and play around with a website, and toggle a command prompt with the `:CocCommand command-here`. And that's just the surface of what you can do with Coc!




