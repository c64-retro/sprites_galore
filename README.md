# Sprites Galore!
C64 Sprite Editor With Font Conversion, Wash Patterns, and More

## Help

In main window, press "H" to show the help screen.

| Key           | Action                       | Note
|---------------|------------------------------|-----
| H             | Show Help Screens            | [SPACE] For Next Page / Exit
| [CURSOR-KEYS] | Move Plotter                 |
| [SPACE]       | Plot / Erase Pixel           |
| [JOY-DIR]     | Move Plotter                 |
| [JOY-BUTTON]  | Plot / Erase Pixel           |
| V             | Set Joystick Velocity        |
| 1             | Increment Draw Color #1      |
| 2             | Increment Draw Color #2      | Multi-Color Mode
| 3             | Increment Draw Color #3      | Multi-Color Mode
| 4             | Increment Bacground Color    |
| M             | Toggle Multi-Color Mode      |
| C             | Toggle Draw Color (1 - 3)    | Multie-Color Mode
| G             | Toggle Grid                  |
| I             | Invert Sprite Pixels         | Simple Bit Toggle
| P             | Goto Sprite Page             | Pages 0 - 499
| +             | Next Sprite Page             | Wraps After 499
| -             | Previous Sprite Page         | Wraps After 0
| X             | Toggle X-Expand              |
| Y             | Toggle Y-Expand              |
| [SHIFT] X     | Flip Sprite Horizontal       |
| [SHIFT] Y     | Flip Sprite Vertical         |
| [SHIFT] [CLR] | Clear Sprite Data            | Current Page Only
| R             | Toggle Scroll Wrap/Clear     |
| F1            | Scroll Sprite Right          | Earases Left If Wrap Off
| F2            | Scroll Sprite Left           | Earases Right If Wrap Off
| F3            | Scroll Sprite Up             | Earases Bottom If Wrap Off
| F4            | Scroll Sprite Down           | Earases Top If Wrap Off
| F7            | Save Sprite To Buffer        | Slots 1 - 8
| F8            | Load Sprite From Buffer      | Overwrites Current Sprite
| W             | Save Wash Pattern            | Slots 1 - 8
| [SHIFT] W     | Apply Wash Pattern           | Paints Empty Pixels
| F6            | View Sprite on Blank Screen  | Keys: 1, 2, 3, 4, M, X, Y. [SPACE] To Exit
| D             | Change Current Drive         |
| F5            | Directory Listing            | 
| L             | Load Sprites From Disk       |
| S             | Save Sprites To Disk         |
| F             | Convert Disk Font To Sprites | Starts At Page 200.  For Y = 3, Bottom Row Clipped
| [SHIFT] F     | Convert ROM Font To Sprites  | Starts At Page 200.  For Y = 3, Bottom Row Clipped

## Instructions for Assembly

Using the [CC65](https://www.cc65.org/) assembler suite:

    cl65 -t c64 -C c64-asm.cfg  --start-addr '$1000' -o sprites_galore.prg sprites_galore.a65

## Output of Assembly

    sprites_galore.prg

NOTE: `sprites_galore.prg` is uncrunched.  To execute it as-is:

    load"*",8,1
    sys 8192

