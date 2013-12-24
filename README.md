# iman: illumos man page viewer

iman is a tiny script for viewing illumos man pages from OS X.  Man pages are
fetched from http://illumos.org/man.  By default, iman looks for the "links"
browser and uses that to render the page.  If "links" isn't found, it uses
"open" to open the URL in your default browser.

**iman [-s SECTION] NAME**

Use `iman` like man, except that only the "-s" option is supported.

Load the `read` man page (defaults to section 1: command-line programs):

    iman read

Specify section 2 (system calls) instead:

    iman -s2 read

Thanks to Josh Clulow for the illumos.org man page viewer.
