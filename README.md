Linux Machine ID
================

Get the unique machine ID on Linux.

This script has been tested with:

  - Ubuntu >= 18.04
  - Fedora >= XX.XX

Installation
------------

### Quick Install

    curl --silent https://raw.githubusercontent.com/PHLAK/linux-machine-id/master/machine-id \
        | sudo tee /usr/local/bin/machine-id

### Manual Installation

  1. Download or clone this repo
  2. Copy `machine-id` to a location on your `$PATH` (e.g. `/usr/local/bin`)
  3. Ensure `machine-id` is executable

      `chmod +x /usr/local/bin/machine-id`

Usage
-----

After following the instructions above you can run `machine-id` from a terminal
to output the machine ID in various formats.

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
