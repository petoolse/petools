# PE Tools History

## PE Tools v1.9

### [1.9.762.2018](https://petoolse.github.io/petools/Announce-EN)
`4 Apr 2018`
- [ ] Fixed bug in `Add New Section`: [Virtual Address Alignment](https://github.com/petoolse/petools/issues/3)


### [1.9.712.2018](https://petoolse.github.io/petools/Announce-EN)
`30 Mar 2018`

#### Principal Changes

##### Fixes

> Primarily, new release is about bug fixes. There are lot of things fixed including memory leaks and program logic. Be warned, sometimes new bugs are replacing old ones, but we had worked hard to bring you bug-free release without introducing new bugs (we really hope so).

##### New Features

Some nice new features are added to make your experience more visible and comfortable:

- [x] Brand new **Entropy View** (approximately detect packing status, presence of encrypted data) with two modes: Curve and Histogram;
- [x] New disassembler engine (previously it was CADt by Ms-Rem, then Mediana by mika0x65 and now it's diStorm by Gil Dabah) has now resulted in x86-64 (64 bit) disasm in addition to x86 (32 bit);
- [x] Load Config Directory (`IMAGE_LOAD_CONFIG_DIRECTORY`) support with new additional values and sizes (non-standard sizes);
- [x] Display of Structured Exception Handlers in Config directory;
- [x] Certificates (Security Directory) removal (with all certificates);
- [x] File System Redirector (Windows-on-Windows, WoW) support;
- [x] Edit functionality in hex-editor;
- [x] Correct process list display in modern OS;
- [x] Display x86-64 (64 bit) processes in process list;
- [x] DLL Characteristics dialog;
- [x] PE Sniffer (Signs.txt) are translated to PEiD format.

### A whole bunch of small but useful features

- [x] Link files support (.lnk);
- [x] Debug directory info: PDB name, GUID, POGO types, VC types;
- [x] Disasm call/jmp direction (up / down relative to current offset);
- [x] Copy and Save menus in disasm and hex-editor dialogs;
- [x] Copy options in hex-editor: C source, Editor display, hex values (raw bytes);
- [x] Shortcuts in Copy menu in hex-editor;
- [x] Fill Block dialog in в hex-editor: fill with values; XOR, OR, AND, NOT operations supported;
- [x] Sections Editor shows zero-based section number (useful with files with many unnamed sections);
- [x] Default action for double click: opening corresponding dialogs without context menu by default;
- [x] Values `OperatingSystemVersion` and `SubsystemVersion` are automatically updated to conform maximum number of sections for specific OS when increasing number of sections;
- [ ] Correct calculation and fix of certain header sizes;
- [x] Detection of many int3 opcodes to interrupt fast disasm;
- [ ] Correct relocation table removal with fix of corresponding flags;
- [ ] Serious bugs fixed in File Location Calculator (FLC);
- [ ] Import adder: fixed library name truncation bug;
- [x] Auto close of Admin privilege warning.

#### Get high

High-DPI display modes supported including 192 DPI:
- [x] DPI modes supported and tested: 96, 120, 144, 192
- [x] Graphics redrawn:
  - [x] Main Application Icon
  - [x] Logo
  - [x] Toolbar icons

#### Cleanup

Outdated and unnecessary features removed:
- [ ] Old update system removed;
- [ ] Plugins removed (old plugins had very basic API set with only 2 functions);
- [x] Number of external libraries reduced;
- [x] Modules with similar functionality merged.

## PE Tools v1.8

`2017` _internal_
- TODO: Update history

## PE Tools v1.7

### 1.7.100 alfa 4

`18 Jan 2012` _internal_

- [x] Default values when adding new section: `SizeOfRawData = 0x200` and `VirtualSize = 0x1000`
- [x] Option to set `PE Sniffer` database: API `SetDataFile`
- [x] `PESniffer` database is now loaded from `PESniffer.dll` location path, not from calling app path

### 1.7.100 alfa 3

`18 July 2011` _internal_
- [ ] Fixed bug in `import adder`

### 1.7.100 alfa 2

`28 Nov 2009` _internal_

- [x] Open file in `PE Editor` by double click in process list
- [x] Edit section header by double click on section name in `Sections Editor`.
- [x] When adding section from zero-sized file, 'Fill with zero' method chosen.
- [x] Added more predefined section names (`Borland`, `UPX`)
- [x] Open configuration dialog from command line: `/CFG` option. No need to wait main `PE Tools` window loading.
- [x] The `/CFG` parameter may be added to open configuration dialog before rebuilding file: `/REBUILDPE File.exe /CFG`
- [x] "Keep file time" option for `PE Rebuilder`
- [x] New manifest for modern OS

### 1.7.100 alfa 1

`27 Nov 2009` _internal_
- [x] Build using `Visual Studio 2008`
- [x] Small additions and changes

## PE Tools v1.6

_internal_
- [ ] Small bug-fixes
- [x] Source code refactoring

## PE Tools v1.5

### 1.5.800.2005 RC7

`14 May 2006` _internal_

- [ ] Many bugs fixed
- [x] `PTDS SDK` added


### 1.5.700.2005 RC6

`11.10.05` _internal_

- [ ] `Section Editor` bug fixed
- [ ] Bug in resiurce handler fixed
- [x] Small internal changed
- [x] New version of CADt `disassembler` by Ms-Rem

### 1.5.400.2003

`08 Dec 2003` _Xmas Edition_

- [x] Added `Generic OEP Finder`
- [x] `DumpFixer` added to `Section Editor`
- [x] New signatures added (Tnx: .Cryorb/dyn!o/DeMoNiX/Aster!x/FEUERRADER)
- [x] `PE Sniffer` code is optimized
- [x] Ability to increment `SizeOfHeaders` added
- [x] New plugin added - `Recover UPX` by Quantum
- [x] Added `ToolBar`
- [x] All options are saved in `INI` file now
- [x] Control elements are changed a little in `Sections Editor` and `Directory Editor`
- [x] Examples of plugins in` MASM32/Delphi` are added to `SDK`
- [x] Signature creation utility (`SignMan`) is now distributed along with the main package
- [x] `PE Tools` won't allow to edit `IMAGE_DOS_HEADER` if offset on `IMAGE_OPTIONAL_HEADER` is less than size of - `IMAGE_DOS_HEADER`
- [x] New version of update module (UUpdateSystem.dll)
- [x] `MMF` functions are re-written
- [ ] Bug in `File Location Calculator` fixed (Tnx: cyberbob)
- [ ] Bug in `Kill Section` (from file) fixed
- [ ] Small bug in process dumper fixed
- [ ] Bug in `Task Viewer` removed
- [ ] Bug in `Break & Enter` removed
- [ ] Bug with options saving is removed
- [x] PE Tools now works fine on `Win95` (Tnx: Lepton)
- [x] Sections processing algorithm is significantly changed

## PE Tools v1.4

### 1.4.419.2003

`21 Mar 2003`
- [ ] Interface bugs fixed
- [x] Program can now correctly dump processes protected by `tElock`
- [x] uinC Update System added

## PE Tools v1.3

### 1.3 Build 60

`09 Dec 2002`
- [ ] Fixed bugs in sections processing code

### 1.3 Build 54

`24 Aug 2002`
- [x] Now program automatically chooses a method of opening of files (Full access or Read-Only)
- [x] The program displays section which has entrypoint
- [x] `Drag-Drop`` support added
- [x] Additional functions to work with sections are added
- [x] Code for PE files processing is re-written again
- [ ] Bugs related to section processing fixed

### 1.3

`01 June 2002`
- [x] The program is renamed to PE Tools (Thanks to NiFi)
- [x] Now the program can edit DOS-compatible header
- [x] New features: backup copy creation and opening of files in read-only mode
- [x] Procedure of identification of PE-files was considerably improved
- [ ] Bug with opening files fixed

## PE Tools v1.2

`13 May 2002`
- [ ] Some bugs fixed
- [ ] Program does not open Read-Only files
- [x] Sources are provided with binaries

## PE Tools v1.1

`07 May 2002`
- [x] First public release. `GUI` application
- [ ] Bug with sections fixed
- [x] Functions for working with PE files are completely re-written
- [x] Preservation of changes warning is added
- [x] Process of command line is added
- [x] Additional types of processors in Advanced Information

## PE Tools v1.0

`03 Feb 2002`
- [x] Initial `console` version `never distributed`

[back](./)
