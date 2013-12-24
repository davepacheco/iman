# iman: illumos man page viewer

iman is a tiny script for viewing illumos man pages from OS X.  Man pages are
fetched from http://illumos.org/man.  By default, iman looks for the "links"
browser and uses that to render the page.  If "links" isn't found, it uses
"open" to open the URL in your default browser.

## Usage

Use `iman` like man, except that only the "-s" option is supported:

**iman [-s SECTION] NAME**

e.g.,

`iman read`: loads `read` from section 1 (command-line programs)
`iman -s2 read`: loads `read` from section 2 (system calls)
