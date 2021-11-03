# suckless.tags

### Script to go to a tag and move master window to a tag with ease.

#### Suckless.tags can now be used to change volume, brightness, keyboard backlight and toggle touchpad

*There has been an update. Pay attention to the focused tags in the status bar in this video.*

https://user-images.githubusercontent.com/85027668/139577611-26936d4e-2119-45e1-b5f5-585639aac186.mp4

I've placed the script under /usr/local/bin

```
const char *tagcmd[]      = {"st", "-f", "Fira Code:size=13", "-n", "tag", "-g", "36x6",  "-e", "tags", NULL };
```
I created a scratchpad that calls the script.

### Prerequisites

- setup scratchpad for the popup

- amixer for changing volume

- brightnessctl for changing brightness

- Place the touchpad_toggle script under /usr/local/bin

- Make sure both the scripts are executable(chmod +rwx /path/to/script)

    - dwm ;)

    It'd be better to map the command to toggle the scratchpad to a dedicated key instead of combination to reduce number of keypresses.

### The script prompts you for the action.

    - Press g to go to a workspace and m to move the master window to a workspace.

    - If you chose g then now choose an alphabet or a number to go to that workspace.

    - If you chose m then now choose an alphabet or a number to move master to that workspace.

    - If you chose v then press j to reduce volume, k to increase or any other key to quit.

    - If you chose b then press j to reduce brightness, k to brightness or any other key to quit.

    - To quit out of the entire program when you're in the first menu, press q.


    __NOTE:__

    - _The script uses xdotool so please change the key names in the script accordingly._

    - _You can use alphabets as well as numbers._

    - _To use pulseaudio instead of alsa, just follow the commented instructions in the script.
