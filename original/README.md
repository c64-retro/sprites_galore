# Sprites Galore!
Original Files and disassembler configurations.

## Files

| File                          | Description 
|-------------------------------|------------
| `sprites-galore-runnable.prg` | Original program as distributed.  Crunched and runnable.
| `sprites-galore-1000.prg`     | Original program, uncrunched.  Range = $1000 - $3500. Entry point = $2000
| `sprites-galore.info`         | DA65 configuration for initial disassembly.
| `sprites-galre.sym`           | DA65 labels for initial disassembly.

## Instructions for Disassembly

    da65 -i sprites_galore.info

## Output of Disassembly

    sprites_galore-1000.a65

