# objmv - A tool to rename sections

[libhermit-rs](https://github.com/hermitcore/libhermit-rs) is a [unikernel](http://unikernel.org/), where the kernel is linked as library to the application.
To separate the kernel from the application, `objmv` is used to rename all code, data and bss sections to `.ktext`, `.kdata` and `.kbss`.
It based on the tool `objcopy` and is only tested on Linux.

```bash
$ # rename all sections
$ objmv libtest.a
```
