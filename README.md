# WinLUKS project

WinLUKS is basically the LUKS (Linux Unified Key Setup) implementation to
Windows 10 and above.

## What about LibreCrypt/FreeOFTE

LibreCrypt (former FreeOFTE) is a project that lacks the drivers to interact
with LUKS-enabled devices, meaning that the project is, unfortunately, useless
in the current state. As its own maintainer stated: fixing the issues with the
code would involve re-architecturing the drivers and rewriting the core DLLs
from scratch.

Since the overall code is unchanged for more than 7 years and no other
opensource software seems to be available to handle LUKS on Windows, this seems
a good opportunity to create a new one.

## Disclaimer

I sincerely have no clue how to implement LUKS nor Windows Drivers. This is the
first time I'm touching Windows native API, everything I've done so far was
directly on Linux userspace, using default GNU glibc and Linux Kernel
interfaces or even Kernel code. Also, the coding style I'll start using will be
entirely based on K&R style: from naming to calling conventions.

With that in mind, I hope this project can get to the point where it's useful
to someone.

## Features

The feature we have already implemented:

- [ ] [LUKS specification v1](https://mirrors.edge.kernel.org/pub/linux/utils/cryptsetup/LUKS_docs/on-disk-format.pdf)
- [ ] [LUKS specification v2](https://gitlab.com/cryptsetup/LUKS2-docs/-/blob/main/luks2_doc_wip.pdf)
- [ ] _Windows device driver_ (I have no clue)

