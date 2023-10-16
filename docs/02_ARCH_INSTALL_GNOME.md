# Installation of Arch Linux Gnome

## Prerequisites

1. You have the [Base Installation](01_ARCH_INSTALL_BASE.md) done.
2. We will be using yay (aur helper) for ease of use. you can just use pacman command directly or if its aur package then use any aur helper.

## Installation Steps

- Install the gnome & gnome extra package

    ```sh
    yay -S gnome gnome-extra
    # if asked for between jack2 or pipewire-jack choose pipewire-jack (I use pipewire so i choose that. If you are using something else then choose that.)
    # if asked for between pipewire-media-session or wireplumber choose wireplumber (I use wireplumber so i choose that. If you are using something else then choose that.)
    # for fonts i choose default you can choose whatever you wish
    ```

- Enable the display manager so gnome can start automatically on startup

    ```sh
    sudo systemctl enable gdm.service
    ```

- Reboot your system

    ```sh
    reboot
    ```

- Enable Fractional Scaling in Gnome (Not working on my laptop but works on my PC. Try it)

    ```sh
    sudo pacman -S dconf-editor
    ```

  - in org.gnome.mutter -> expermimental features -> scale-monitor-framebuffer
- If you are into tiling like i am pop-shell is the way to go on gnome (i specially like it enable disable functionality)

    ```sh
    yay -S gnome-shell-extension-pop-shell-git  
    ```

## Some UserFriendly Gnome Extensions & Apps

- Install Extension Manager from Flathub. (You can find it in Software Center provided by GNOME)
- AppIndicator and KStatusNotfierItem Support
- Caffine
- Lock Keys
- Arch Linux updates Indicator
- Blur My Shell
- Clipboard Indicator
- Vitals
- User Avatar in Quick Settings
- Show Desktop Button
