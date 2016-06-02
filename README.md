# BMXNG-Packs

Contains prebuild packs of "BMX-NG" for various OS.


All files are created as following:
(all sources are taken from https://github.com/bmx-ng)
- compile bcc / bmk / makedocs / docmods for the platform
- copy current brl.mod / pub.mod / maxmod2.mod
- to compile "MaxIDE"
  - maxgui.mod is fetched and copied to the mods
  - github.com/maxmods/bah.mod is fetched and copied to the mods (only
    gtkmaxgui.mod / gtkwebgtkhtml.mod are needed)
  - maxide-sources are fetched
  - MaxIDE is compiled for the platform via

    Linux32: ./bmk makeapp -r -g x86 path/to/maxide.bmx

    Linux64: ./bmk makeapp -r -g x84 path/to/maxide.bmx

    ...
- compress everything into one archive for easy downloadability
