# Ultimate-Ventoy

This repo mirrors my own USB file structure, the root of this repo is the root of the Ventoy exfat partition.

I dont include the theme files. But provide a link for direct download from the creator on the folder where those theme files should be put on!


step-by-step setup
1. Install Ventoy on a USB Stick for multiboot capabilities(https://www.ventoy.net/en/doc_start.html)
2. Create ventoy folder on root
3. Create Ventoy.json on ventoy folder
4. Clone my Ventoy.json or read documentation(https://www.ventoy.net/en/plugin_entry.html) to make your own!
5. Insert autounattend.xml on root directory
6. Populate root with all the .iso files you want, and name them acording to the ISO list on Ventoy.json.
7. OPTIONAL: configure a theme using: https://www.ventoy.net/en/plugin_theme.html

My theme.txt in included in its appropriate folder: ventoy/theme/ventoy/

PS: It is possible to store data/general arbitrary data as well on that drive using the remaining space! just make a new folder for it!

Ventoy.json settings file expects the following names for your ISOs:
- Windows11(25H2).iso
- Windows10(22H2).iso
- Ubuntu-24.0.4.3.iso
- Kali-Linux_Live.iso
- HBCD.iso
- memtest.iso (memtest86+)

Add and subtract disks as needed!
Change expected names and list order on ventoy.json under the "key" and "list" entries respectively

  Custom autounattend.xml: A "Client-Control" focused Windows installation.

    Automated & Debloated: Removes shovelware/sponsored apps while keeping the Microsoft Store functional, giving the user the option to install them back.

    Privacy First: Disables Telemetry, "Tailored Experiences," and silent background installs.

    Diagnostic Ready: Pre-configures AppLocker in Audit Mode for easy post-install troubleshooting.

    Security Measures: Disables a few legacy drivers and functions from windows that might pose security risks for the average user.

    Fully commented! Remove, Disable or Add whatever you want with no confusion on what each line does!
    
  If the default location for this script is at root, it will always be pulled by a windows installation no matter what.

Once booted the drive should look like this:
<img width="1023" height="766" alt="image" src="https://github.com/user-attachments/assets/7f8acacf-8ba0-4f9b-ab1f-07ca87ded9a3" />

