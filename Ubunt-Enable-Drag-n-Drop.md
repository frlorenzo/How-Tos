# Enable Drag & Drop


## Install gnome extensions app

```
sudo apt install gnome-tweak-tool
```

Open the **Extensions** app and disable Desktop Icons.


## Install nemo

```
sudo apt install nemo
```

Open **Startup Applications**. Click the Add button on the top right to add a new entry. In the edit startup program, locate the file **nemo-desktop** (which /usr/bin/nemo-desktop). 

- Name: Nemo Desktop
- Command: /usr/bin/nemo-desktop
- Comment: Enable Drag & Drop for Desktop

When you log back in you should be able to drag and drop things to and from your desktop again.



## References

https://sudofry.com/2020/06/02/restore-drag-drop-in-ubuntu-20-04/
