# fumbbl_linux

If you don't know what [Fumbbl](https://fumbbl.com) is, this won't be too useful.

You need to install java for first this to work and run the Fumbbl client.

Fumbbl's horribly outdated, closed-source client still relies on Java Web Start to start a match; getting this to run on Linux is non trivial.

This script is a hack to just download the jars and run, based on the .jnlp file served out by Fumbbl.com.

Usage: 

```
chmod +x fumbbl
./fumbbl /path/to/ffblive.jnlp
```

It will download all the jars in the JWS file to the current directory. To avoid re-downloading the client files, use `./fumbbl -noupdate ffblive.jnlp`.

*Note*: It's a zsh script; hopefully you have `/bin/zsh` handy?
