<div aling="center">
    <img src="./dwm.png" alt="dwm-logo" width="195" height="90"/>

    # Dynamic window manager
</div> 
---
This is my personal fork of dwm. It focus in productivity, minimalism and stability with nice user interface.

<details>
    <summary> Click to see the list of patches applied in my ricing </summary>
    
    - alwaysCenter
    - attachBottom
    - autoStart
    - moveStack
    - pertag
    - status2d
    - vanityGapps [Includes bottom stack, gridmode, fibonnaci layouts and more]
    - warp

</details>

## Prerequisites
You need to have Xorg for launching dwm and devel tools.

For to do: Adding cli lines for dependencies installation
<details>
    <summary>Arch</summary>
</details>

<details>
    <summary>Debian/ubuntu</summary>
</details>

<details>
    <summary>RedHat/Fedora</summary>
</details>



> [!NOTE]
> You may want to have your dwmw folder in a specific folder, so you can always go back if you made configuration changes before compilation. In any case this dwm ricing works well out of the box.

## Installation

```sh
git clone https://github.com/CarlosR759/dwm-carlos.git && cd dwm-carlos
```
```sh
sudo make clean install
```

- A dwm.desktop file will be placed in `/usr/share/xsessions` for login managers.

- If you want to run it by tty then be sure to have xinit script installed and setup your .xinitrc well. After everything at the end of the .xinitrc file append `dwm`

> [!TIP]
> - By default you launch terminals with <kbd>SUPER/Windows</kbd>+<kbd>Enter</kbd> If you don't have alacritty go to config.h and edit the file to have your desired terminal.

> - You can kill your dwm session with <kbd>SUPER/Windows</kbd>+<kbd>Shift</kbd>+<kbd>Q<kbd>
> - For keybindings changes made it in config.h

## Faq
Did you have  the same rice for wayland in dwl ? 

Answer: No I dont have it. Since I want my system to be stable for work intentions, i made the decision to use dwm. Maybe in the future I could make it, but only if I see that dwl + patches is stable and the switching from Xorg is a better choice for productivity.

What compositor did you use for your animations ? 

Answer: I use the default picom made by yshui which is the default in many distros. FT-Labs and PiJulius picoms are also great adn with more animations, but doesn't have the same support as yshui picom and are experimental. So for stability reasons I decided to use yshui picom, so less fancy animations but stable and comfy system.

How can I get the power, reset, lock and suspend bottoms at the end of the gif video ?

Answer: Just get my dot files or use the content of my rofi content in your .config folder. This also can be applied to my picom config if you like the animations.

How can I get the centered menu in  your gif video ? 

Answer: Just go to my dmenu repo and install it




