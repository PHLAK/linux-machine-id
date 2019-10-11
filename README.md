Linux Machine ID
================

Get the unique machine ID on Linux.

This script has been tested with:

  - Ubuntu >= 18.04
  - Debian >= 10
  - Fedora >= 30

For more information on Linux machine IDs see
<http://man7.org/linux/man-pages/man5/machine-id.5.html>

Installation
------------

### Quick Install

    curl --silent https://raw.githubusercontent.com/PHLAK/linux-machine-id/master/machine-id \
    | sudo install /dev/stdin /usr/local/bin/machine-id

### Manual Installation

  1. Download or clone this repo
  2. Copy `machine-id` to a location on your `$PATH` (e.g. `/usr/local/bin`)
  3. Ensure `machine-id` is executable

      `chmod +x /usr/local/bin/machine-id`

Usage
-----

After following the instructions above you can run `machine-id` from a terminal
to output a unique machine ID in various formats.

    $ machine-id
    8654c188be4386abe2ae2c0e0a682681f4cf2b33d71ac6cb8f6fba50d09735c8

By default the command returns a sha256 hash of the device ID found in
`/etc/machine-id`. You can use the `--raw` option to return the actual machine
ID and the `--short` option to get the short version of the ID.

    Usage: machine-id [OPTION]...
    Get the machine's unique ID.

    OPTIONS:
    -h, --help     Print this help dialogue
    -r, --raw      Retuns the raw machine ID
    -s, --short    Return a short (7 character) ID

Changelog
---------

A list of changes can be found on the [GitHub Releases](https://github.com/PHLAK/linux-machine-id/releases) page.

Troubleshooting
---------------

Please report bugs to the [GitHub Issue Tracker](https://github.com/PHLAK/linux-machine-id/issues).

Copyright
---------

This project is licensed under the [MIT License](https://github.com/PHLAK/linux-machine-id/blob/master/LICENSE).
