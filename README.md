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

you can also just use my setup by cloning the theme folder to the ventoy folder that is on root, alongside the .json

PS: It is possible to store data/general arbitrary data as well on that drive using the remaining space! just make a new folder for it!

Settings files expect the following content:
- Windows11(25H2).iso
- Windows10(22H2).iso
- Ubuntu-24.0.4.3.iso
- Kali-Linux_Live.iso  (Networking/Security/DataRecovery)
- HBCD.iso
- memtest.iso  (test memory state without booting into host OS)

You dont need to only use these or even have all of them, change expected names and list order on ventoy.json key and list entries respectively

The autounattend.xml file allows for the installation of a persistent debloated Windows, that only gets compromised on major updates.
No more ads, auto-silent installs, shovelware recommendations. Microsoft store and app functionalities unaffected, it lets you choose what you actually want for your windows. 
Left Copilot in because it might break the system nowadays unfortunately....
