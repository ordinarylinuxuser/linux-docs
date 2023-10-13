# Installation of Arch Linux Gnome

## Prerequisites

1. You have the [Base Installation](01_ARCH_INSTALL_BASE.md) done.
2. We will be using yay (aur helper) for each of use. you can just use pacman command directly or if its aur package then use any aur helper.


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