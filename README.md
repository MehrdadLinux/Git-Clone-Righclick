# Git-Clone-Righclick
Add git clone to your context menu or right-click mouse operation

How do it faster
Copy this script and save it in file
``` bash
#!/bin/bash

clip=$(xclip -o -selection clipboard)
folder_name=$(echo "$clip" | grep -oP '(?<=\/)[^\/]+(?=\.git)')
git clone "$clip" "$PWD/$folder_name"
```

Gnome scripts
GNOME Files, formerly and internally known as Nautilus, is the official file manager for the GNOME desktop Nautilus script is an executable shell script that is placed in a special scripts directory so that the Nautilus graphical shell can find it. This allows you to extend the functionality of the file browser to do just about anything.

     ~/.local/share/nautilus/scripts/
How it works?
Copy script in Gnome scripts path and change file permission

    chmod a+x [yourscript]
Righclick on folder and select yourscript done

Do you have a question?


