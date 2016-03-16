# ULF

ULF stands for "Update Localizable Strings" and it is a Perl Script for merging
new translation phrases from one .strings file to another.

## What does it do?

The script reads both, the language file and the base file, into associative
arrays using the translation key as identifier for a translation. Then it
prints all translations of base file, but if the translation exists in the
langague file the language file version of the translation is printed.
Therefore existing translations stay unchanged. This algorythm removes needless
translations.

## Usage

    ulf <lang_file> <base_file> [<out_file>]

## Examples

    ulf en.lproj/Localizable.strings Base.lproj/Localizeable.strings
merges new phrases from 'Base' to 'en' and prints the result to `stdout`

    ulf en.lproj/Localizable.strings Base.lproj/Localizeable.strings en.lproj/Localizable.strings
merges new phrases from 'Base' to 'en' and writes the result to 'en'

# License

MIT

Copyright (c) 2014-2016 Johannes Bauer

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.