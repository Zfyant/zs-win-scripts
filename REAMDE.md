# README - Cap Windsurf RAM usage

 - Note: MD files can be parsed nice for both human & code, which is how you see it now. Find a nice MD parsing extension in your browser to view a cleaner version of this README.md.

## Requirements
 - 1. Downloading & Installing 3rd party zipped software `Procgov`
 - 2. Limited know-how of using a text editor to write a small script
 - 3. This script or your own variant & targeting correct locations

## Contents
 - 1. Download `Procgov` from its website
 - 2. Create `Windsurf_CapRam.vbs` from provided example.
 - 3. [optional] Create VBS file shortcut (custom icon / start menu entry)


## How To

### 1. Download `Procgov`
- Use your search engine of choice to find `procgov` and download its zip/exe from the Github sources-page/website.
- Extract/Install to your location of choice, notate this location somewhere.

### 2. Create `Windsurf_CapRam.vbs`
- Copy this script to your own new file, I named mine `Windsurf_CapRam.vbs`
```
Set WshShell = CreateObject("WScript.Shell")
' Build the full ProcGov command:
cmd = """C:\Program Files\procgov\procgov.exe"" --maxmem 4G --nogui --recursive -- ""C:\Program Files\Windsurf\Windsurf.exe"""
' Run it hidden (0 = window style hidden, False = don't wait)
WshShell.Run cmd, 0, False
```
- Correct the file paths if you've installed either your script and/or program in another location.
- Save & Test via double-clicking.

### 3. Run from Start Menu (Allows pinning)
- `Right-click drag` or `Right-click > Send To > Desktop` to create a shortcut.
- For best practice, ensure this gets placed in the Windsurf folder.
- Right click > Properties > Change Icon > Browse: Windsurf.exe > OK > OK
- Open the Start folder: Press `Win + R` > `shell:Start Menu` > Programs
- Copy the newly created and styled shortcut to this folder.
- New you can find it in the start menu and even pin it for easy open.

## Enjoy~!
