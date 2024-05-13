```
As a GPT ina CLI mood, you are Restarting...

Award Modular BIOS v4.51PG, An Energy Star Ally
Copyright (C) 1984-98, Award Software, Inc.

Main Processor  : Intel Pentium II 400MHz
Coprocessor     : Built-in 

Floppy Drive A: 1.44M, 3.5 in.
Floppy Drive B: None

Pri Master : IBM-DPTA-372050 
Pri Slave  : None
Sec Master : ATAPI CD-ROM 32X
Sec Slave  : None

Memory Cache: 512KB Pipelined Burst SRAM

Extended Memory: 256MB
Base Memory    : 640KB  

  Date (mm:dd:yy) : Fri 12/04/1998
  Time (hh:mm:ss) : 09:15:22

  Halt On: All Errors But Keyboard

  Floppy Drive Seek: Enabled
  Floppy Drive Swap: Disabled 
  Primary Display  : VGA/EGA

  Virus Warning    : Disabled
  CPU Internal Cache : Enabled
  Quick Power On Self Test: Enabled

  Boot Sequence:
   Diskette Drive
   Hard Drive
   ATAPI CD-ROM
   
Press DEL to enter SETUP
Press F8 for BBS POPUP

...

Starting MS-DOS...

Microsoft(R) MS-DOS(R)  Version 6.22
(C)Copyright Microsoft Corp 1981-1994

C:\>TYPE CONFIG.SYS
DEVICE=C:\DOS\HIMEM.SYS
DEVICE=C:\DOS\EMM386.EXE RAM
DOS=HIGH,UMB
FILES=40
BUFFERS=20
STACKS=9,256
DEVICEHIGH=C:\DOS\ANSI.SYS
SHELL=C:\DOS\COMMAND.COM C:\DOS /E:1024 /P

C:\>TYPE AUTOEXEC.BAT
@ECHO OFF
PROMPT $p$g
PATH C:\DOS;C:\WINDOWS
SET TEMP=C:\DOS
C:\DOS\SMARTDRV.EXE /X
C:\DOS\MSCDEX.EXE /D:MSCD001 /L:D
LH C:\DOS\DOSKEY
LH C:\DOS\MOUSE.COM

C:\WINDOWS\win

C:\>ECHO Starting DOS Menu...

DOS Menu v1.0

1. Windows 3.11
2. Microsoft Word
3. Microsoft Excel
4. Notepad
5. File Manager
6. Exit to DOS

Enter your choice: 1

Starting Windows 3.11...

Microsoft Windows 3.11
Copyright (c) 1985-1993 Microsoft Corp.

'''
.-----------------------. 
                       /|        Windows        |\
                      / |                       | \
                     /  |    Version 3.1    _   |  \
                    /   |                  (_)  |   \
                   /    |      _  _  _  _       |    \
                  /     |     (_)(_)(_)(_)_     |     \
                 /      |    _             (_)   |      \
                /       |   (_)                  |       \
               /        |                        |        \
              /         |  Microsoft Windows 3.1 |         \
             /          |                        |          \
            /           |                        |           \
           /            |                        |            \
          /             |________________________|             \
         /                                                      \
        /                                                        \
       /                                                          \
      /                                                            \
     /                 .--------------------------------.          \
    /                 /|             Welcome to         |\         \
   /                 / |           Windows 3.11         | \        \
  /                 /  |                                |  \       \
 /                 /   |       Please wait while        |   \      \
/                 /    |        Windows loads...        |    \     \
                 /     |                                |     \
                /      |                                |      \
               /       |                                |       \
              /        |________________________________|        \
             /                                                   \
            /                                                     \
           /                                                       \
          /                                                         \
         /                                                           \
        /                                                             \
       /                                                               \
      /                                                                 \
     /                                                                   \
    /                                                                     \
   /                                                                       \
  /                                                                         \
 /                                                                           \
/                                                                             \
-------------------------------------------------------------------------------
Program Manager File Options Window Help

|_|  Main  |_|

| - | |\    Exit Windows | Yes | No | y
Exiting to MS-Dos...
```
```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'primaryColor': '#ffaa00', 'primaryTextColor': '#ffaa00', 'primaryBorderColor': '#ffaa00', 'lineColor': '#ffaa00', 'secondaryColor': '#ffaa00', 'tertiaryColor': '#ffaa00', 'clusterBkg': 'none', 'clusterBorder': 'none', 'fontSize': '0px'}}}%%
graph TD
    A["Boot Process Start"] -->|BIOS Check| B["Award Modular BIOS v4.51PG"]

    B --> C["Main Processor: Intel Pentium II 400MHz"]
    B --> D["Coprocessor: Built-in"]
    B --> E["Floppy Drive A: 1.44M, 3.5 in."]
    B --> F["Primary Master: IBM-DPTA-372050"]
    B --> G["Secondary Master: ATAPI CD-ROM 32X"]
    B --> H["Memory: 256MB Extended, 640KB Base"]

    H --> I["System Date & Time"]
    I -->|Date| J["Date (mm:dd:yy): Fri 12/04/1998"]
    I -->|Time| K["Time (hh:mm:ss): 09:15:22"]

    I --> L["Boot Device Sequence"]
    L --> M["1. Diskette Drive"]
    L --> N["2. Hard Drive"]
    L --> O["3. ATAPI CD-ROM"]

    I --> P["BIOS Settings"]
    P --> Q["Halt On: All Errors But Keyboard"]
    P --> R["Quick Power On Self Test: Enabled"]
    P --> S["Primary Display: VGA/EGA"]

    A --> T["Starting MS-DOS"]
    T --> U["Microsoft MS-DOS Version 6.22"]

    U --> V["Load CONFIG.SYS"]
    V --> W["DEVICE=C:\\DOS\\HIMEM.SYS"]
    V --> X["DEVICE=C:\\DOS\\EMM386.EXE RAM"]
    V --> Y["FILES=40, BUFFERS=20, STACKS=9,256"]

    U --> Z["Load AUTOEXEC.BAT"]
    Z --> AA["SMARTDRV and MSCDEX Drivers"]
    Z --> AB["Load High DOSKEY, MOUSE.COM"]

    U --> AC["Command Prompt C:\\>"]
    AC --> AD["DOS Menu v1.0"]
    AD -->|Choice: 1| AE["Starting Windows 3.11"]

    AE --> AF["Microsoft Windows 3.11"]
    AF --> AG["Program Manager Loaded"]

    AF --> AH["Exiting to MS-DOS"]

    subgraph BIOS
        B --> C
        B --> D
        B --> E
        B --> F
        B --> G
        B --> H
    end

    subgraph DateTime
        I --> J
        I --> K
    end

    subgraph BootSequence
        L --> M
        L --> N
        L --> O
    end

    subgraph BiosSettings
        P --> Q
        P --> R
        P --> S
    end

    subgraph DosLoad
        V
        W
        X
        Y
        Z
        AA
        AB
    end

    subgraph Windows
        AE --> AF
        AF --> AG
        AF --> AH
    end
```
