# st - simple terminal (k_lar's build)

st is a simple terminal emulator for X which sucks less.  

My build is fairly minimal, since I don't need much from my terminal apart from that it needs to
be fast, render UTF-8 and not consume a ton of resources. 

**Patches:**
- Alpha
- Boxdraw
- Clipboard
- Gruvbox
- Fix keyboard input

This build **DOES NOT** support scrollback unlike most forks/builds.
I'm using tmux, because it handles history/scrollback better than st's scroll patches, as it's
super janky and weird in my opinion.  

I'm using a font called BlexMono (IBM Plex Mono Nerd Font). It's available in the AUR, otherwise
you can find it here: TODO: Add link to BlexMono Github  


## Installation

Install with: (in source directory)
```console
> sudo make install
```

You can uninstall st with: (in source directory)
```console
> sudo make uninstall
```


## Misc (from old README)

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

