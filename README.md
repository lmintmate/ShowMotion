# ShowMotion

Ever hammered the {`w`,`W`,`b`,`B`,`e`,`E`,`ge`,`gE`,`;`,`,`} keys to finally pass over the location you were aiming for?  
ShowMotion is a tiny vim plugin to highlight the potential landing places when moving:

* by words with {`w`,`W`,`b`,`B`,`e`,`E`,`ge`,`gE`}.
* by chars with {`f`,`F`,`t`,`T`,`;`,`,`}

Somewhat inspired by the EasyMotion plugin, this one is only aimed at providing cues about where you'll land, not allowing to select a specific landing place. The pleasant consequence of this is it doesn't break your moving flow, which was the motivation for writing it.

 Demo: https://imgur.com/sWUqiF3

## Installation:

Plugin Manager  | Add to your `/.vimrc`
--------------- | --------------------------------------------------
Vim Plug        | `Plug 'lmintmate/ShowMotion'`
NeoBundle       | `NeoBundle 'lmintmate/ShowMotion'`
Vundle          | `Plugin 'lmintmate/ShowMotion'`
 
 ## Configuration

Add these word-motion settings to your vimrc, either the first or the second group (depending on your preferences):  

    "*** Highlights both big and small motions
    nmap w <Plug>(show-motion-both-w)
    nmap W <Plug>(show-motion-both-W)
    nmap b <Plug>(show-motion-both-b)
    nmap B <Plug>(show-motion-both-B)
    nmap e <Plug>(show-motion-both-e)
    nmap E <Plug>(show-motion-both-E)
    nmap ge <Plug>(show-motion-both-ge)
    nmap gE <Plug>(show-motion-both-gE)

    "*** Only highlights motions corresponding to the one you typed
    nmap w <Plug>(show-motion-w)
    nmap W <Plug>(show-motion-W)
    nmap b <Plug>(show-motion-b)
    nmap B <Plug>(show-motion-B)
    nmap e <Plug>(show-motion-e)
    nmap E <Plug>(show-motion-E)
    nmap ge <Plug>(show-motion-ge)
    nmap gE <Plug>(show-motion-gE)

Add these character-motion settings to your vimrc:  

    "Show motion for chars:  
    nmap f <Plug>(show-motion-f)
    nmap t <Plug>(show-motion-t)
    nmap F <Plug>(show-motion-F)
    nmap T <Plug>(show-motion-T)
    nmap ; <Plug>(show-motion-;)
    nmap , <Plug>(show-motion-,)


Known limitations:

* `E` fails on highlighting the last character in the line

Thanks:
 
* IRC: #vim, sakkemo, bairui, Raimondi and many others
* Github: itchyny, haya14busa, Pyrohh
