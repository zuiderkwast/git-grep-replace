git-grep-replace
================

This script combines `git grep` with a global replacement (`s///g`) within each
of the matching files.

```
Usage: git grep-replace [ OPTIONS ] PATTERN [ REPLACEMENT ]

The script combines 'git grep' with a global replacement within each of the
matching files.

Options:

  -P  --perl-regexp    Perl regexp.
  -F  --fixed-strings  Fixed strings.
  -i  --ignore-case    Case insensitive matching.
  -D  --delete         Delete matching lines. No REPLACEMENT.
  -d  --dry            Dry run. Changes written to files with '~~~' suffix.
  -v  --verbose        More printouts.
  -h  --help           Print help and exit.

Either -P or -F must be given. REPLACEMENT must be given except if -D is
specified.
```

The script is capable of Perl regular expressions and fixed strings, but not
simple nor extended regular expressions, so either `-P` or `-F` must be given.

Installation
------------

Copy the script to e.g. `/usr/local/bin/` and do `chmod +x` if necessary.
