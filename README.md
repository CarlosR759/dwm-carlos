<div align="center">
  <img src="./dwm.png" alt="dwm-logo-bordered" width="195" height="90"/>

  \\# Dynamic window manager

</div>

---
This is my personal fork of dwm. It focus in productivity, minimalism and stability with nice user interface.

<details>
  <summary> Click to see the list of patches applied in my dwm ricing </summary>
  
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
You need to have Xorg for launching dwm and devel tools for compiling. Git is not mandatory for installation so you can delete it form the command if you want.

<details>
  <summary>Arch</summary>

  ```sh
  sudo pacman -S base base-devel xorg git
  ```
</details>

<details>
  <summary>Debian/ubuntu</summary>

  ```sh
  sudo apt install build-essential xorg git
  ```
  
</details>

<details>
  <summary>RedHat/Fedora</summary>

  ```sh
  sudo dnf install @base-x gitt && sudo dnf groupinstall "Development Tools" "Development Libraries"
  ```
</details>



> [!NOTE]
> - You may want to have your dwm folder in a specific folder, so you can always go back if you made configuration changes before compilation. In any case this dwm ricing works well out of the box.
> - If you want to have dmenu centered check my dmenu repo at 
> - If you want to use dwm with xinit, check if your xorg installation came with xinit, most of the time it does, but if you don't have it you can install it by searching for the package xinit in your distribution.
> - If you want the picom animations check my dotfiles repo. Animations uses experimental features from picom "https://picom.app/#_animations" because I use geometry-change. If you want a system with no posible bugs maybe you want to use it without the animations field.

## Installation

```sh
git clone https://github.com/CarlosR759/dwm-rice.git && cd dwm-rice
```

```sh
sudo make clean install
```

- A dwm.desktop file will be placed in `/usr/share/xsessions` for login managers.

- If you want to run it by tty then be sure to have xinit script installed and setup your .xinitrc well. After everything at the end of the .xinitrc file append `dwm`

> [!TIP]
> - By default you can launch terminals with <kbd>SUPER/Windows</kbd>+<kbd>Enter</kbd> If you don't have alacritty go to config.h and edit the file to have your desired terminal.
> - You can kill your dwm session with <kbd>SUPER/Windows</kbd>+<kbd>Shift</kbd>+<kbd>Q</kbd>
> - For keybindings changes made it in config.h

## FAQ

#### Did you have  the same rice for wayland in dwl ? 

\<details>

No I dont have it. Since I want my system to be stable for work intentions, i made the decision to use dwm. Maybe in the future I could make it, but only if I see that dwl + patches is stable and the switching from Xorg is a better choice for productivity.
</details>

#### What compositor did you use for your animations ? 

\<details>

I use the default picom made by yshui which is the default in many distros. FT-Labs and PiJulius picoms are also great and with many more animations, but doesn't have the same support as yshui picom and are experimental. So for stability reasons I decided to use yshui picom, so less fancy animations but stable and comfy system.
\</details>

#### How can I get the power, reset, lock and suspend bottoms at the end of the gif video ?

\<details>

Just get my dot files or use the content of my rofi content in your .config folder. This also can be applied to my picom config if you like the animations.
</details>

#### How can I get the centered menu in your gif video ? 

\<details>

Just go to my dmenu repo and install it
</details>
