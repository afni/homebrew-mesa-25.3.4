# mesa-25.3.4

This is a patch to install a slightly older version mesa on Macs. 
suma does not work with versions 26.0.3 until 26.2.0 at least on Intel and ARM Macs.

```
brew tap afni/mesa-25.3.4
brew install mesa@25.3.4

rm /opt/homebrew/opt/mesa 
ln -s /opt/homebrew/Cellar/mesa@25.3.4/25.3.4 /opt/homebrew/opt/mesa
brew link --overwrite mesa@25.3.4
```

You may also need an update to the expat library and to the MacOS (26.3->26.4).

```
brew update expat
```

Issues are being submitted to homebrew and mesa projects for a long-term resolution.

Much thanks to Pete Molfese for this contribution!
