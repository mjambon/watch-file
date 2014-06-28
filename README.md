watch-file
==========

Rerun a command when a file changes.

This provides automatic refresh functionality to software that doesn't
have it built in.

Example
-------

You can use the following command to view a file `file.out`
whose content changes:

```sh
$ watch-file file.out less file.out
```

`watch-file` runs `less file.out`. It inspects `file.out`
for changes periodically, and when a change is detected
the current `less` process is terminated and a new one is created.
