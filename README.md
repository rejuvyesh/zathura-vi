[pwmt's `zathura`](http://pwmt.org/projects/zathura/), with my customisations. So far:

  - Each window provides an X property, `_ZATHURA_FILEPATH`, describing the
    absolute file-path of the open document. I have `cron` periodically run a 
    [script](https://github.com/fmap/vi-bin/blob/master/cron/dwarf) to save 
    each of these, providing a list from which to restore my session post-reboot.

  - The current page number, coordinates, etc. are written to history upon each
    adjustment. The standard behaviour is for these only to be saved on close
    of the viewer; this change preserves my settings on occasion of `SIGKILL`.
