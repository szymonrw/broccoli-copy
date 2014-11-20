# broccoli-copy

Merges and copies trees. Tracks file changes and copies only changed
files, also removes those removed in source trees.

## Usage

    var tree = copy([<tree1>, <tree2>], options)

Options:

- `extensions`: array of allowed extensions
- `filter`: regular expression for filtering paths
- `dest_dir`: copy files to a subdirectory

## Example

Example brocfile:

    var copy = require("broccoli-copy");

    module.exports = copy(["styles", "app"], {
      extensions: ["css", "js"]
    });

## COPYING

MIT License.
