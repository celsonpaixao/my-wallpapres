
# Como divionar o wallpaper dinamico

### Primeiro encontrar o arquivo xml da distro

Encontrar o arquivo xml da distro

```bash
  sudo find /usr/share/gnome-background-properties -type f -name "*wallpapers.xml"
```

### Editar o arquivo xml eencontrado

O codigo anterior irá retornar a localização do seu aqrivo xml, então só iremos abir ele no vs code ou num outro editor de exto

```bash
 sudo code /usr/share/seu-caminho/seu-arquivo-wallpapers.xml      
```
ou 
```bash
code /usr/share/seu-caminho/seu-arquivo-wallpapers.xml      
```
ou 

Também pode user o gedit

```bash
sudo gedit /usr/share/gnome-background-properties/zorin-default-wallpapers.xml   
```
### Inserir o novo wallpaper dimanico

```bash
 <wallpaper>
    <name>Nome para o wallpaper</name>
    <filename>o caminho</filename>
    <options>zoom</options>
    <pcolor>#000000</pcolor>
    <scolor>#000000</scolor>
    <shade_type>solid</shade_type>
  </wallpaper>
   
```

