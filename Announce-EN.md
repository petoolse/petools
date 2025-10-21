# Meet the new release of good old-fashioned PE Tools

It's been years since NEOx released latest public version of PE Tools in 2006, so you may have decided that PET is already dead, but it came back from the dead for a while in 2018!


## Principal Changes

### Fixes

> Primarily, new release is about bug fixes. There are lot of things fixed including memory leaks and program logic. Be warned, sometimes new bugs are replacing old ones, but we had worked hard to bring you bug-free release without introducing new bugs (we really hope so).


### New Features

Some nice new features are added to make your experience more visible and comfortable:

- [x] Brand new **Entropy View** (approximately detect packing status, presence of encrypted data) with two modes: Curve and Histogram;
!["Entropy"][screens.entropy]
- [x] New disassembler engine (previously it was CADt by Ms-Rem, then Mediana by mika0x65 and now it's [diStorm][distorm.gh] by Gil Dabah) has now resulted in x86-64 (64 bit) disasm in addition to x86 (32 bit);
!["Disasm"][screens.disasm]
- [x] Load Config Directory (`IMAGE_LOAD_CONFIG_DIRECTORY`) support with new additional values and sizes (non-standard sizes);
- [x] Display of Structured Exception Handlers in Config directory;
- [x] Certificates (Security Directory) removal (with all certificates);
- [x] File System Redirector (Windows-on-Windows, WoW) support;
- [x] Edit functionality in hex-editor;
- [x] Correct process list display in modern OS;
- [x] Display x86-64 (64 bit) processes in process list;
- [x] DLL Characteristics dialog;
- [x] PE Sniffer (`Signs.txt`) are translated to PEiD format.


### A whole bunch of small but useful features

- [x] Link files support (.lnk);
- [x] Debug directory info: PDB name, GUID, POGO types, VC types;
- [x] Disasm call/jmp direction (up / down relative to current offset);
- [x] Copy and Save menus in disasm and hex-editor dialogs;
- [x] Copy options in hex-editor:
	- C source
	- Editor display
	- hex values (raw bytes)
- [x] Shortcuts in Copy menu in hex-editor;
- [x] **Fill Block** dialog in в hex-editor: fill with values; `XOR`, `OR`, `AND`, `NOT` operations supported;
- [x] Sections Editor shows zero-based section number (useful with files with many unnamed sections);
- [x] Default action for double click: opening corresponding dialogs without context menu by default;
- [x] Values `OperatingSystemVersion` and `SubsystemVersion` are automatically updated to conform maximum number of sections for specific OS when increasing number of sections;
- [x] Correct calculation and fix of certain header sizes;
- [x] Detection of many `int3` opcodes to interrupt fast disasm;
- [x] Correct relocation table removal with fix of corresponding flags;
- [x] Serious bugs fixed in **File Location Calculator** (FLC);
- [x] Import adder: fixed library name truncation bug;
- [x] Auto close of Admin privilege warning.


### Get high

High-DPI display modes supported including 192 DPI:
- [x] DPI modes supported and tested: 96, 120, 144, 192
- [x] Graphics redrawn:
	- [x] Main Application Icon
	- [x] Logo
	- [x] Toolbar icons


### Cleanup

Outdated and unnecessary features removed:
- [x] Old update system removed;
- [x] Plugins removed (old plugins had very basic API set with only 2 functions);
- [x] Number of external libraries reduced;
- [x] Modules with similar functionality merged.


### Other changes

Full list of changes:
- [HISTORY][petools.history.gh]

Many other small things are fixed or added (not all are listed), so it's a good way to study new features by downloading new release.


### Links

Project site on Github:
- [petoolse.github.io/petools][petools.web.gh]

PE Tools project news:
- [@petoolse][twitter]


### DOWNLOAD

- [github.com/petoolse/petools/releases][petools.releases.gh]

--
- [Jupiter][jupiter.gh]
- [PainteR][painter.gh]

`2018.03.30`

[back](./)


[distorm.gh]: https://github.com/gdabah/distorm

[screens.entropy]: screens/PETools-Screens-Entropy.gif
[screens.disasm]: screens/PETools-Screen-Disasm-diStorm.png

[petools.web.gh]: https://petoolse.github.io/petools
[petools.releases.gh]: https://github.com/petoolse/petools/releases
[petools.issues.gh]: https://github.com/petoolse/petools/issues
[petools.history.gh]: https://petoolse.github.io/petools/HISTORY

[jupiter.gh]: https://github.com/upiter
[painter.gh]: https://github.com/pr701

[twitter]: https://x.com/petoolse
