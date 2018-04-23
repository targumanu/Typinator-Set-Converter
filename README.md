<p align="center"><img src="/icon.png" width="128" height="128"></p>

# Typinator Set Converter

Alfred file action for converting Typinator sets to Alfred snippet collections

The workflow supports only Typinator sets exported as plain text files.<br/>
(.tyset and .typubset are proprietary binary formats and cannot be read)
 
When converting Typinator snippets, the workflow replaces Typinator’s cursor marker `{^}` with Alfred’s cursor placeholder `{cursor}`.<br/>
Other Typinator markers are not supported.
 
The workflow uses [OneUpdater](https://github.com/vitorgalvao/alfred-workflows/tree/master/OneUpdater) for automatic updates.

### Installation

Download and install the [latest release](https://github.com/targumanu/Typinator-Set-Converter/releases/latest).

### Usage

- Select one or more Typinator snippet sets exported as plain text files
- Invoke Alfred’s file actions pane `⌥⌘\`
- Select `Convert Typinator Sets`
- Press `↵`

### Options

The configuration options are set using the workflow’s environment variables.

All the configuration variables, except “prefix” and “suffix”, are “pseudo-Boolean”:
- “True”, “yes” or “1” are case-insensitively interpreted as `true`
- Any other value or no value means `false`

| Configuration Variable | Functionality                                                |
| :--------------------- | :----------------------------------------------------------- |
| `customicon`           | Use the workflow’s custom icon for created snippet collections |
| `dontautoexpand`       | Disable automatic expansion for all snippets                 |
| `dontcompress`         | Do not compress the folder containing the converted snippets.<br />This option may be useful, if you want to make some manual changes to converted snippets.<br />To compress manually, just zip the folder and change its extension from `zip` to `alfredsnippets` |
| `noprefix`             | Do not use any prefixes for converted sets.<br />Even if all keywords in a set have the same prefix, they will remain unchanged, and no prefix will be added to this set’s preferences. |
| `nosuffix`             | Do not use any suffixes for converted sets.<br />Even if all keywords in a set have the same suffix, they will remain unchanged, and no suffix will be added to this set’s preferences. |
| `prefix`               | Force the specified prefix for all converted snippet sets.<br />The specified prefix will be added to the preferences of converted snippet sets.<br />If a snippet keyword has the specified prefix, it will be removed from the keyword.<br />For example, if you set `prefix` to “//”, then “//keyword” will become “keyword”. |
| `suffix`               | Force the specified suffix for all converted snippet sets.<br />The specified suffix will be added to the preferences of converted snippet sets.<br />If a snippet keyword has the specified suffix, it will be removed from the keyword<br />For example, if you set `suffix` to “//”, then “keyword//” will become “keyword”). |

----------

Support the developer   [<img src='https://upload.wikimedia.org/wikipedia/commons/5/53/PayPal_2014_logo.svg' height='18' alt='Support via Paypal'>](https://paypal.me/targumanu)
