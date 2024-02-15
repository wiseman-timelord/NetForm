# InfoEventMon

### Status
Alpha; Consolidating, Performancer and WhaGoWan and maybe some other half-developed ones, into a single program "InfoEventMon", for system monitoring, device info and recent events...
1. Progress submenu options for "Device Information" to completion; Options on Submenu have been refined to, System, Graphics, Sound... 
- Issue with finding text in report, this will require test scripts, to see what is going on when retrieving applicable lines.
- However it ends up working, I will need to implement this into the functions. 
- remember to try include some limited drive info in system, see how much space is left.
2. When it produce the "SystemEvents.Log", or the other one, it should then prompt "Select; Open = O, Back = B: "...
- if open then open the file with notepad.
- the other text on the page near the bottom needs a little work also.
- consider using the ".\cache" folder.

## Description
InfoEventMon Will become a tool for, System Information, Device Monitoring, System Events, in one place, it will all be done through cmdlets, so, dont expect much.

### Features
**CPU/Network Monitoring:** Monitor the performance of your, Processor or Network, see `Preview` section below.
**Application/System Events:** Export recent events to a relevantly relating `ProgramEvents.Txt/SystemEvents.Txt`.  

### Preview
The Main Menu...
```
=========================( PerfEventMon )=========================











                     1. Performance Monitor,

                     2. Device Information,

                     3. Recent Events Report.










---------------------------------------------------------------
Select, Options = 1-3, Exit = X: :

```
- Monitoring Options (both screens)...
```
=========================( InfoEventMon )=========================

CPU Name: AMD Ryzen 9 3900X 12-Core Processor
Maximum Threads: 24
Maximum Clock Speed: 3801MHz
Current Clock Speed: 3793MHz
CPU Usage: 9.6%

---------------------------------------------------------------
Select; Back = B
Refreshing In 5 Seconds...

...

=========================( InfoEventMon )=========================

NIC Name: Realtek PCIe GbE Family Controller
Status: Up
Speed: 1 Gbps
IPv4 Address: XXX.XXX.XXX.XXX
Download Rate: 15.4 KB/s
Upload Rate: 13.5 KB/s
Discards Total: 0
Errors Total: 0

---------------------------------------------------------------
Select; Back = B
Refreshing In 5 Seconds...

```
- Production of System Events reports...
```

=========================( InfoEventMon )==========================

Requesting System Events..
..System Events Received.

Exporting Report to SystemEvents.Log..
..SystemEvents.Log Report Exported.

Check Event Report File; Returning To Menu...


```


## Usage
1. Unpack the program to a sensible location, sensible locations do not include, "C:\Program Files" or "C:\Program Files(x86)", though it may work in those locations.
2. Run `InfoEventMon.Bat`, select `Option 1`, the `main.ps1` script will then load.
3. Navigate the menus, select your options, as you prefer. 
4. Navigate `Back` to the main menu, then `Exit` the program, then `Exit` the Launcher.

### Requirements
(compatibility ranges require calculation)
- Windows based environment with, Scripting Host and Batch/PowerShell Support, Enabled.
- .Net 2.0+ - Breaking a loop is impossible without this, check out [SystemConfig](https://github.com/wiseman-timelord/SystemConfig) for offline install of .net 3.5 if your having issues. (this project is not currently complete)
- DirectX - For detailed device information, of course you can use DxDiag, but my program refines the info.
- PowerShell - If your having issues, then upgrade your PowerShell, or alternatively install, [PWSH 7.4 MSI](https://github.com/PowerShell/PowerShell/releases/download/v7.4.0/PowerShell-7.4.0-win-x64.msi) or [PWSH 7.4](https://github.com/PowerShell/PowerShell/releases/tag/v7.4.0) (and make sure its on PATH). (compatibility ranges require calculation) 

## Notation
- This is a, consolidation and update and upgrade, of multiple of my other programs.

### Development
- TBA

## Disclaimer
This software is subject to the terms in License.Txt, covering usage, distribution, and modifications. For full details on your rights and obligations, refer to License.Txt.
