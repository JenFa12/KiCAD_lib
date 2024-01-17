KiCad Library
This repository contains the library, which are used in KiCad.<br>
The following README explains how to set up KiCad with the lib and how to add you librarys to the repository. 

## KiCad
[KiCad Download-Link](https://www.kicad.org/download/)

### Setup

1. clone repo: 
    ```
    git clone https://github.com/JenFa12/KiCAD_lib.git
    ```

2. Settings -> configure paths
3. Add 3 paths:
    | Name              | Path                            |
    | :---              |    :----:                       |
    | KiCAD_3D_DIR        | {kicad-lib-path}/packages3D |
    | KiCAD_SYMBOL_DIR    | {kicad-lib-path}/symbols |
    | KiCAD_FOOTPRINT_DIR | {kicad-lib-path}/footprint |

### Symbol Editor
Library:
- Existing Library: File -> Add Library -> Global -> {kicad-lib-path}/symbols -> thu-{bibgroub}-tht.lib -> symbol.kicad_sym
- New Library: File -> New Library -> Global -> {kicad-lib-path}/symbols -> thu-{bibgroub}-tht.lib -> {New_Library}.kicad_sym

Symbol:
- Existing Symbol: Select existing lib -> File -> Import Symbol -> Global -> {kicad-lib-path}/symbols -> thu-{bibgroub}-tht.lib -> {symbol}.lib
- New Symbol: Select existing lib -> File -> New Symbol

### Footprint Editor
Library:
- Existing Library: File -> Add Library -> Global -> {kicad-lib-path}/footprints -> thu-{bibgroub}-tht.pretty
- New Library: File -> New Library -> Global -> {kicad-lib-path}/footprints -> thu-{bibgroub}-tht.pretty

Footprint:
- Existing Footprint: Select existing lib -> File -> Import Symbol -> Global -> {kicad-lib-path}/footprints -> thu-{bibgroub}-tht.pretty -> {symbol}.kicad_mod
- New Footprint: Select existing lib -> File -> New Symbol

### 3d Model
- Save 3D-Modle into {kicad-lib-path}/packages§D -> thu-{bibgroub}-tht.3dshapes -> {modelname}.step
- Add Model in the Footprint Editor to the footprint: Press Key E -> 3D-Model -> Add 3D-Model
