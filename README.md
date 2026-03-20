# Ultimate-Ventoy

This repo mirrors my own USB file structure. i dont include the theme files.
these folders are to be located on the Root of the Ventoy formatted USB

step-by-step setup
1. Install Ventoy on a USB Stick for multiboot capabilities(https://www.ventoy.net/en/doc_start.html)
2. Create ventoy folder on root
3. Create Ventoy.json on ventoy folder
4. Clone Ventoy.json or read documentation(https://www.ventoy.net/en/plugin_entry.html)
5. Insert autounattend.xml on root directory
6. Populate root with all the .iso files you want
7. OPTIONAL: configure a theme using: https://www.ventoy.net/en/plugin_theme.html

My theme.txt in included in its appropriate folder: ventoy/theme/ventoy/

PS: It is possible to store data/general arbitrary data as well on that drive using the remaining space! just make a new folder for it!

Settings files expect the following content:
- Windows11(25H2).iso
- Windows10(22H2).iso
- Ubuntu-24.0.4.3.iso
- Kali-Linux_Live.iso
- HBCD.iso
- memtest.iso

You dont need to only use these or even have all of them, change expected names and list order on ventoy.json key and list entries respectively

  Custom autounattend.xml: A "Client-Control" focused Windows installation.

    Automated & Debloated: Removes shovelware/sponsored apps while keeping the Microsoft Store functional.

    Privacy First: Disables Telemetry, "Tailored Experiences," and silent background installs.

    Diagnostic Ready: Pre-configures AppLocker in Audit Mode for easy post-install troubleshooting.
