![](img/petools-logo-blue-128.png)

**PE Tools** - [portable executable](https://en.wikipedia.org/wiki/Portable_Executable) (PE) manipulation toolkit.

## Table of contents

- [Description](#description)
- [Features](#features)
    - [PE Editor](#pe-editor)
    - [File Location Calculator](#file-location-calculator-flc)
    - [PE Files Comparator](#pe-files-comparator)
    - [Process Viewer and Manager](#process-viewer-and-manager)
    - [PE Dumper](#pe-dumper)
    - [PE Rebuilder](#pe-rebuilder)
    - [PE Sniffer](#pe-sniffer)
- [System Requirements](system-requirements)
- [Limitations](#limitations)
- [To do](#to-do)
- [What's new](#whats-new-in-recent-major-releases)
- [Creators](#creators)
- [Contacts](#contacts)


## Description

> **PE Tools** let you actively *research* PE files and processes.
> `Process Viewer` and PE files `Editor`, `Dumper`, `Rebuilder`, `Comparator`, `Analyzer` are included.
> **PE Tools** is an *oldschool reverse engineering tool* with a long history since `2002`.

## Features

### PE Editor

- PE and DOS Headers **Editor**
- PE Sections **Editor**
- PE Directory _Viewer_ and **Editor**
- Export Directory **Editor**
- Import Directory **Editor**
- Resource Directory _Viewer_
- Exception Directory _Viewer_
- Relocation Directory _Viewer_
- Debug Directory _Viewer_
- TLS Directory **Editor**
- Load Config Directory **Editor**
- Bound Directory **Editor**

### File Location Calculator (FLC)

- Virtual Address
- Relative Virtual Address
- Raw File Offset

## PE Files Comparator

- Side-by-side comparison of headers and characteristics of two PE files

## Process Viewer and Manager

- Show basic process information
- Show process modules

## PE Dumper

- Running process dumper
    - Full Dump
    - Partial Dump
    - Region Dump
- ~~Dumper Server (accessible via Dumper Server SDK)~~

## PE Rebuilder

- Dump Fixer
- Relocation Wiper
- Resource Directory Rebuilder
- PE file Validation
- Imports Binder
- ImageBase Changer

## PE Sniffer

- Signature analysis of PE files
- Packer detection

## HEX Editor

- HEX Editor available in:
    - `Section Editor` via section context menu
    - Every `Data Directory` in `Directory Editor`

## Plugins

- ~~PE Tools `Plugin SDK` available~~

## What's new in recent major releases

### PE Tools v1.9

#### Entropy View
- Entropy Viewer available in:
    - Main `PE Editor` dialog
    - `Section Editor` via section context menu
    - `File Location Calculator (FLC)` for both compared files

#### 64-bit Disassembler
- [diStorm](https://github.com/gdabah/distorm) `v3.3.4`
- Shows `jmp / call` direction

#### Load Config Directory Editor

- `IMAGE_LOAD_CONFIG_DIRECTORY` support
- Additional Load Config Directory values and size support (non-standard sizes)

#### High-DPI display modes support

- 192 DPI supported
- `DPI` modes supported and tested: `96`, `120`, `144`, `192`
- Graphics redrawn:
    - Main Application Icon
    - Logo
    - Toolbar icons


#### Bug-fixes and minor changes

See [HISTORY](HISTORY)


## System Requirements

- Latest tested Operating System: [Windows 10](https://en.wikipedia.org/wiki/Windows_10)
- Supported Windows versions: [Windows 10](https://en.wikipedia.org/wiki/Windows_10), [Windows 8.1](https://en.wikipedia.org/wiki/Windows_8.1), [Windows 8](https://en.wikipedia.org/wiki/Windows_8), [Windows 7](https://en.wikipedia.org/wiki/Windows_7)
- Minimal Operating System: [Windows XP](https://en.wikipedia.org/wiki/Windows_XP)
- Administrative rights for `SeDebugPrivilege`
- macOS supported via [Wine](https://www.winehq.org) (tested Wine 2.16)
- [ReactOS](https://www.reactos.org) natively supported (tested Reactos 0.4.5)


## Limitations

- No [large files support](https://en.wikipedia.org/wiki/Large_file_support) (over 4 GB)
- No [ARM disassembler](https://en.wikipedia.org/wiki/ARM_architecture#Operating_system_support) support (ARM architecture supported by [Windows 10 Mobile](https://en.wikipedia.org/wiki/Windows_10_Mobile), [Windows RT](https://en.wikipedia.org/wiki/Windows_RT), [Windows Phone](https://en.wikipedia.org/wiki/Windows_Phone), [Windows IoT Core](https://en.wikipedia.org/wiki/Windows_IoT#Core), [Windows Embedded Compact](https://en.wikipedia.org/wiki/Windows_Embedded_Compact))

## Source code

```C++
throw std::exception(“​PE Tools source code is not available”);
```
- If you want to add some features, write ready-to-use snippet (C/C++) and post it in [Issues](https://github.com/petoolse/petools/issues)

## To do

- [ ] `Win64` version
- [ ] File `Overlay` Analyzer and Extractor
- [ ] `Authenticode` Viewer
- [x] `Rich` Signature Editor
- [ ] `Relocations` Checker
- [ ] Enhance `Debug` Directory Remover: remove debug section if empty
- [ ] [Corkami](https://github.com/corkami/pocs/tree/master/PE/bin) binaries testing and support
- [ ] `.NET Directory` Viewer
- [ ] `External Tools` support (preliminary list):
    - [ ] [x64dbg](https://x64dbg.com)
    - [ ] [Scylla Imports Reconstruction](https://github.com/NtQuery/Scylla)
    - [ ] [Hiew](http://hiew.ru)
    - [ ] [r2](https://github.com/radare/radare2)
    - [ ] [Resource Hacker](http://www.angusj.com/resourcehacker)
- [ ] `Structures Export` to readable formats like `JSON` / `YAML`
- [ ] `Crypto` tools (`hash`, `decryption` / `decryption`)
- [ ] `ARM` disassembler (far-far-away)


## Licensing

See [LICENSE](LICENSE)


## Creators

- NEOx [[uinC](http://uinc.ru/files/neox/PE_Tools.shtml)] - versions up to `1.5`, 2002-2006
- [Jupiter](https://github.com/upiter) - versions from `1.5`, 2007-2018
- PainteR - versions from `1.8`, 2017-2018
- [EvilsInterrupt](https://bitbucket.org/sys_dev/) aka [NtVisigoth](http://ntvisigoth.blogspot.com) - versions from `1.5`, 2012-2014


## Contacts

Feel free to contact via Twitter [@petoolse](https://twitter.com/petoolse).
