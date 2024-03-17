# Commodore-C64-Games---Source-Code-and-Rebuild

Purpose:
  Start with an old Commodore C64 game disk which is as close to the original as possible (*.g64/*.nib) including the copy protection.
  Produce a commented assembler listing which reassembles to an exact copy of the originla binary.
  Make the source as variable as possible to allow any kind of modifications (relocate data areas/code).

  Sometimes add some own ideas to the game soures code for fun and as a proof of concept (is the extracted source code is really veariable?).

Project:
  All sources come as Notpad++ projects

Utilities used:
  ASM: 64tass
  Disassembler: 65xxdis
  Disk manager: DirMaster
  Emulator: WinVice
  NIB converter: NibTools

Directory structure:
  dox - additional documentation
  npp - Notepadd++ modification instructions/language files/toolbar icons
  C64
    tools
      64tass
      DisAsm
    asm
      Projects
        < npp_project >.xml
        Data
          inc - C64 system includes
          
          originals - Game sources
            < c64_game >
              asm - source code
              d64 - C64 disk files
              dis - disassemblies
              inc - game includes
              lst - assembler listings
              prg - binaries
              xtra - additional files
                
              all.bat - call both, 64tass and 65xxdis
              asm.bat - call 64tass
              dis.bat - call 65xxdis
          mods - Modified games
            < modified_game >
              same structure as above
