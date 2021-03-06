1.5 (2013-08-07)
---------------

* workaround camomile raising the wrong exception for encoding
  failures
* add more default keybindings

1.4 (2013-03-26)
----------------

* added `C-b`, `C-f`, `C-h`, `M-p`, `M-n` by default
* fix a segfault when running utop in an emacs terminal buffer

1.3 (2012-10-08)
----------------

* fix the bindings for `C-n` and `C-p`
* binds `C-h` to delete-prev-char

1.2 (2012-07-30)
----------------

* better handling of newlines in read-line (avoid square selection bug)
* add a module for managing history
* use camomile for character encoding (remove iconv dependency)
    * include generated tables for color mappings to speed up the build
    * Windows fixes
        * use unicode version of IO console functions
        * better rendering method for read-line

1.1 (2011-08-06)
----------------

* fix a blinking problem on OS-X
* bind the `kill-{prev,next}-word` editing actions
* bind the undo action
* add doc for edition actions
* add `LTerm_key.to_string_compact` to print keys like emacs
* use `Zed_input` for key bindings instead of hash tables
* add support for macros
* add the break action to interrupt read-line
* add manual pages
* allow to get the current pending key sequence in read-line
* make the `LTerm_read_line.term` class more flexible
