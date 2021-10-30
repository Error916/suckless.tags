# suckless.tags
Script to go to a tag and move master window to a tag with ease.

https://user-images.githubusercontent.com/85027668/139530565-f1d6e37d-d922-455f-aa74-736cb4e04103.mp4

I've placed the scripts under /usr/local/bin

const char *tagcmd[]     = {"st", "-f", "Fira Code:size=13", "-n", "tag", "-g", "36x6",  "-e", "workspace", NULL };
const char *gotocmd[]     = {"st", "-f", "Fira Code:size=13", "-n", "goto", "-g", "36x6",  "-e", "goto", NULL };

I created two scratchpads that call the script.

By default the workspace script moves the master window to the tag you want. And then takes you to that workspace.

The script uses xdotool so please change the key names in the script accordingly.

You can use alphabets as well as numbers.

