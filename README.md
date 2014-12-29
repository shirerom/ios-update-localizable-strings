ULF
===

ULF stands for "Update Localizable Strings" and it is a Perl Script for merging new translation phrases from one .strings file to another.

Usage
---

    ulf <lang_file> <base_file> [<out_file>]

Examples
---

    ulf en.lproj/Localizable.strings Base.lproj/Localizeable.strings
merges new phrases from 'Base' to 'en' and prints the result to `stdout`

    ulf en.lproj/Localizable.strings Base.lproj/Localizeable.strings en.lproj/Localizable.strings
merges new phrases from 'Base' to 'en' and writes the result to 'en'

