 # Blender
```bash
wget -c https://ftp.nluug.nl/pub/graphics/blender/release/Blender2.83/blender-2.83.0-linux64.tar.xz #update-link
tar -xvf blender*.tar.xz
rm -rfv $HOME/.local/share/blender/
mv blender*/ $HOME/.local/share/blender/
rm -rfv blender*.tar.xz
mkdir -pv $HOME/.local/share/applications
cp -rfv $HOME/.local/share/blender/blender.desktop $HOME/.local/share/applications/
sed -i "s/Exec=blender/Exec=.local\/share\/blender\/blender/g" $HOME/.local/share/applications/blender.desktop
```
[![bashrun](../images/bashrun.png)](br:blender)

![blender](../images/blender.png)