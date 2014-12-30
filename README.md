ULF
===

ULF stands for "Update Localizable Strings" and it is a Perl Script for merging
new translation phrases from one .strings file to another.

What does it do?
---

The script reads both, the language file and the base file, into associative
arrays using the translation key as identifier for a translation. Then it
prints all translations of base file, but if the translation exists in the
langague file the language file version of the translation is printed.
Therefore existing translations stay unchanged. This algorythm removes needless
translations.

Usage
---

    ulf <lang_file> <base_file> [<out_file>]

Examples
---

    ulf en.lproj/Localizable.strings Base.lproj/Localizeable.strings
merges new phrases from 'Base' to 'en' and prints the result to `stdout`

    ulf en.lproj/Localizable.strings Base.lproj/Localizeable.strings en.lproj/Localizable.strings
merges new phrases from 'Base' to 'en' and writes the result to 'en'

