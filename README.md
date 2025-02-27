# Commodore C64 Game Source Code

## Purpose
- Start with an old Commodore C64 game disk which is as close to the original as possible (**g64** or **nib**).
- Include the copy protection.
- Produce a commented assembler listing which reassembles to an exact copy of the originaL binary.
- Make the source as variable as possible to allow any kind of modifications, data area and code relocation.
- Sometimes add some own ideas to the game soures code for fun and as a proof of concept.
- Sometimes add a (simple) level editor.

## Published so far
- **originals**
  - Loderunner                     https://github.com/Piddewitt/Loderunner
  - Championship Loderunner        https://github.com/Piddewitt/Championship_Loderunner
  - The Castles of Dr Creep        https://github.com/Piddewitt/The-Castles-of-Dr-Creep
- **mods**
  - Hansmanns Loderunner           https://github.com/Piddewitt/Hansmanns_Loderunner
  - Hansmanns Castles of Dr Creep  https://github.com/Piddewitt/Hansmanns-Castles-of-Dr-Creep

## Tools used
- Assembler: **64tass**
- Disassembler: **65xxDis**
- Disk manager: **DirMaster**
- Emulator: **WinVice**
- Converter: **NibTools**
  
## Project
- All content comes as a Notepad++ project

## Directory structure
- **dox** - _Additional documentation_
- **npp** - _Notepad++ modification instructions / language files / toolbar icons_
- **C64**
  - **tools**
    - **64tass**
    - **DisAsm**
  - **asm**
    - **Projects**
      - **file:** `npp_project_name.xml`
      - **Data**
        - **inc** - _C64 system includes_
        - **originals** - _Game sources_
          - **c64_game**
            - **asm** - _Source code_
            - **d64** - _C64 disk files_
            - **dis** - _Disassemblies_
            - **inc** - _Game includes_
            - **lst** - _Assembler listings_
            - **prg** - _Binaries_
            - **xtra** - _Additional files_
            - **file:** `all.bat` - _Call both, 64tass and 65xxdis_
            - **file:** `asm.bat` - _Call 64tass_
            - **file:** `dis.bat` - _Call 65xxdis_
        - **mods** - _Modified games_
          - **c64_game**
            - [same structure as above]
