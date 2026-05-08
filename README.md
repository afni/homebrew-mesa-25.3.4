# mesa-25.3.4

This is a patch to install a slightly older version mesa on Macs. 
suma does not work with versions 26.0.3 until 26.2.0 at least on Intel and ARM Macs.

```
brew tap afni/mesa-25.3.4
brew install mesa@25.3.4

rm /opt/homebrew/opt/mesa   # could also use "ln -sfn ...." below 
ln -s /opt/homebrew/Cellar/mesa@25.3.4/25.3.4 /opt/homebrew/opt/mesa
```

Issues are being submitted to homebrew and mesa projects for a resolution.

Much thanks to Pete Molfese for this contribution!
