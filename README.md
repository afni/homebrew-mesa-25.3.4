# mesa-25.3.4

Even after all of that you have to copy over the libGL.1.dylib to the place where mesa-glu wants
```
mkdir -p /opt/homebrew/opt/mesa/lib
ln -sf /opt/homebrew/opt/mesa@25.3.4/lib/libGL.1.dylib /opt/homebrew/opt/mesa/lib/libGL.1.dylib
ln -sf /opt/homebrew/opt/mesa@25.3.4/lib/libGL.dylib /opt/homebrew/opt/mesa/lib/libGL.dylib
```