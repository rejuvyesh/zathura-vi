[pwmt's `zathura`](http://pwmt.org/projects/zathura/), with my customisations. So far:

  - Each window provides an X property, `_ZATHURA_FILEPATH`, describing the
    absolute file-path of the open document. I have `cron` periodically run a
    [script](https://github.com/fmap/vi-bin/blob/master/cron/dwarf) to save
    each of these, providing a list from which to restore my session after
    reboots.

  - The current page number is written to history after each vertical movement.
    The standard behaviour is for this only to be saved on close of the viewer;
    this change preserves my position on occasion of `SIGKILL`.
