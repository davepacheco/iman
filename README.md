# iman: illumos man page viewer

iman is a tiny script for viewing illumos man pages from OS X.  Man pages are
fetched from http://illumos.org/man.  By default, iman uses `curl` to fetch
the page, piping the text to `more` (or `$PAGER`).  The `open` command may
optionally be used to open the URL in your default browser.

**`iman [-o] [-s SECTION] NAME`**

Use `iman` like man, except that only the "-s" option is supported.

Load the `read` man page (defaults to section 1: command-line programs):

    iman read

Specify section 2 (system calls) instead:

    iman -s2 read

Use the "-o" flag to open the page in a browser:

    iman -o -s1M dladm

Thanks to [Joshua M. Clulow](https://twitter.com/jmclulow) for the illumos.org
[man page viewer](https://github.com/jclulow/illumos-webman).
