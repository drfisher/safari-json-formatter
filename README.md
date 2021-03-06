# JSON Formatter

This is a fork of Safari extension by [rfletcher][1] which makes valid JSON documents human-readable.

### Before:
![Before][i1]
### After:
![After][i2]

## Installation
[Download the extension][2] and open it with Safari 5 or higher.

## Usage
Once installed, load any valid JSON document. [This project's most recent
commit][3] makes a good example.

* Click to disclosure triangles to toggle nodes.
* Click to disclosure triangles with Cmd key to toggle nested nodes.

## Extension settings
![Extension settings][i3]

## Version History

### 1.2.2
* Added window opening after click with Cmd key on any url

### 1.2.1
* Added font options
* Small fixies
* Changed "hide/show all" logic

### 1.2
* Code refactoring
* Performance improvements
* Added "hide/show all" ability

### 1.1
* Added folding of arrays, objects and long strings
* Added setting for auto-folding of long strings (default: on)
* Added setting for "long string" threshold (default 512 bytes)
* Added a "toggle formatting" button to switch between formatted and original JSON
* Bug Fixes

## Caveats
The extension aims to produce the same JSON string that's been loaded as input,
but because the original JSON has actually been parsed, some transformation may
occur. In other words, the formatted JSON will always be equivalent to the
original JSON, but in rare circumstances it may not match exactly. The only
known example of this is kind of discrepancy is between number formats -- if the
original JSON contains the numeric value 1e2, for example, the formatted JSON
will display the value 100.

[1]: https://github.com/rfletcher/safari-json-formatter/
[2]: https://cloud.mail.ru/public/d07850f7b26e/JSON_Formatter_1.2.2.safariextz
[3]: http://github.com/drfisher/safari-json-formatter/commit/HEAD.json
[i1]: https://github.com/drfisher/safari-json-formatter/raw/HEAD/etc/images/before.png
[i2]: https://github.com/drfisher/safari-json-formatter/raw/HEAD/etc/images/after.png
[i3]: https://github.com/drfisher/safari-json-formatter/raw/HEAD/etc/images/settings.png