# BMC tpl or tplpre language support in Atom

Adds syntax highlighting and snippets for [tpl](https://docs.bmc.com/docs/display/DISCO111/The+Pattern+Language+TPL) in Atom.

Originally re-made from the [Sublmime text 3 bundle](https://github.com/triaglesis/bmc_tpl).

Build Logic for this package is not included, you can find it in separate [repo](https://github.com/triaglesis/BMC_TPL_IDE)

## Installation:

- Copy 'language-tplpre' to: C:\Users\USER\\.atom\packages\
- Move ".atom-build.yml" to your project root folder.

## Better installation:

Go to settings -> Install -> Search "language-tplpre"

## Use:

####  Set syntax: Ctrl+Shift+L -> type 'tplpre'

![set syntax](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/tpl_set_syntax.gif)

#### Syntax highlighting:

Most of constructions are also checking on integrity,
so if some code will be written on wrong place, highlighting can be broken.

Example:

Pattern from Community Edition:
- ![blocks](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/TPL_Syntax_example_1.png)

Documentation block and tasks highlighted:
- ![docs](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/TPL_Syntax_example_2.png)

Triggers:
- ![regexes](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/TPL_Syntax_example_3.png)

Regex expressions:
(uses python regex grammar from "language-python")
- ![more_regexes](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/TPL_Syntax_example_4.png)


Syntax broken
(highlighting will show it)
- ![syntax_broken](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/tpl_syntax_broken.gif)


#### Autocomplete and Doc links:

For common code blocks and usual constructions autocompletion is available.
It also provide links to reffering documentaion for each function or block on official BMC Doc portal.

Pattern draft example:
- ![pattern_blocks](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/tpl_autocomplete_pattern.gif)

Code constructions usually used:
- ![common_code](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/tpl_autocomplete_versions.gif)

Link to BMC official docs:
- ![docs](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/tpl_autocomplete_model_docs.gif)

Extra developers helping code:
- ![dev_examples](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/tpl_autocomplete_debug.gif)


####  Automation, syntax check, upload pattern, etc:

You should download extra module for TPL Automation
from repo below and attach to build system for Atom.

You can obtain build system in:
- Settings -> Install -> Search "build"
[build system](https://atom.io/packages/build)


TPL Automation: [BMC_TPL_IDE](https://github.com/triaglesis/BMC_TPL_IDE) you can run most development routines automatically.
Atom command templates you can found in Command Palette (Ctrl+Shift+P)

File in project's root - ".atom-build.yml" is example for TPL Automation build,
place it in your project's root folder, where tpl\tplpre files are stored.


![Build](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/TPL_Build_System_example.png)


![Buildresult](https://trianglesis.github.io/blob/master/Atom_language_tpl_pics/BuildSystem_output.png)


Contributions are greatly appreciated. Please fork this repository and open a pull request to add snippets, make grammar tweaks, etc.

### Additional functionality will be added soon in both versions for Sublime Text and Atom.

Fell free to contact me via it@trianglesis.org.ua

Last validation: 2017-08-17
