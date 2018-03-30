# Meet the new release of good old-fashioned PE Tools

It's been years since NEOx released latest public version of PE Tools in 2006, so you may have decided that PET is already dead, but it came back from the dead for a while in 2018!

## Principal Changes

### Fixes

Primarily, new release is about bug fixes. There are lot of things fixed including memory leaks and program logic. Be warned, sometimes new bugs are replacing old ones, but we had worked hard to bring you bug-free release without introducing new bugs (we really hope so).

### New Features

Some nice new features are added to make your experience more visible and comfortable:

- Brand new Entropy View (approximately detect packing status, presence of encrypted data) with two modes: Curve and Histogram;
- New disassembler engine (previously it was CADt by Ms-Rem, then Mediana by mika0x65 and now it's diStorm by Gil Dabah) has now resulted in x86-64 (64 bit) disasm in addition to x86 (32 bit);
- Load Config Directory (IMAGE_LOAD_CONFIG_DIRECTORY) support with new additional values and sizes (non-standard sizes);
- Display of Structured Exception Handlers in Config directory;
- Certificates (Security Directory) removal (with all certificates);
- File System Redirector (Windows-on-Windows, WoW) support;
- Edit functionality in hex-editor;
- Correct process list display in modern OS;
- Display x86-64 (64 bit) processes in process list;
- DLL Characteristics dialog;
- PE Sniffer (Signs.txt) are translated to PEiD format.

## A whole bunch of small but useful features

- Link files support (.lnk);
- Debug directory info: PDB name, GUID, POGO types, VC types;
- Disasm call/jmp direction (up / down relative to current offset);
- Copy and Save menus in disasm and hex-editor dialogs;
- Copy options in hex-editor: C source, Editor display, hex values (raw bytes);
- Shortcuts in Copy menu in hex-editor;
- Fill Block dialog in в hex-editor: fill with values; XOR, OR, AND, NOT operations supported;
- Sections Editor shows zero-based section number (useful with files with many unnamed sections);
- Default action for double click: opening corresponding dialogs without context menu by default;
- Values OperatingSystemVersion and SubsystemVersion are automatically updated to conform maximum number of sections for specific OS when increasing number of sections;
- Correct calculation and fix of certain header sizes;
- Detection of many int3 opcodes to interrupt fast disasm;
- Correct relocation table removal with fix of corresponding flags;
- Serious bugs fixed in File Location Calculator (FLC);
- Import adder: fixed library name truncation bug;
- Auto close of Admin privilege warning.

### Get high

High-DPI display modes supported including 192 DPI:
- DPI modes supported and tested: 96, 120, 144, 192
- Graphics redrawn:
  - Main Application Icon
  - Logo
  - Toolbar icons

### Cleanup

Outdated and unnecessary features removed:
- Old update system removed;
- Plugins removed (old plugins had very basic API set with only 2 functions);
- Number of external libraries reduced;
- Modules with similar functionality merged.

### Other changes

Full list of changes:
- https://petoolse.github.io/petools/HISTORY

Many other small things are fixed or added (not all are listed), so it's a good way to study new features by downloading new release.

### Links

Project site on Github:
- https://petoolse.github.io/petools/

PE Tools project news:
- https://twitter.com/petoolse

### DOWNLOAD

- PE.Tools.v1.9.712.2018.7z
  - https://github.com/petoolse/petools/releases

--
- Jupiter
- PainteR

2018.03.30
