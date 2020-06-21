# fumbbl_linux

If you don't know what Fumbbl is, this won't be too useful.

Fumbbl's horribly outdated, closed-source client still relies on Java Web Start to start a match; getting this to run on Linux is non trivial.

This script is a hack to just download the jars and run, based on the .jnlp file served out by Fumbbl.com.

Usage: 

```
chmod +x fumbbl
./fumbbl update # Download/update the client files
./fumbbl /path/to/ffblive.jnlp
```

To avoid re-downloading the client files, use `./fumbbl -noupdate ffblive.jnlp`.

*Note*: It's a zsh script; hopefully you have `/bin/zsh` handy?
