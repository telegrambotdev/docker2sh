# Docker 2 Shell

This is a simple script to convert a
[Dockerfile](https://docs.docker.com/engine/reference/builder/) to a
shell script that can be executed to replicate the same commands on
any machine or chroot.

[![software by Dyne.org](https://files.dyne.org/software_by_dyne.png)](http://www.dyne.org)

Its primary use is coupled with the [Devuan
SDK](https://git.devuan.org/sdk) where we use Docker to prototype and
then this script to "toast" the prototype inside a Devuan blend.

Another use is inside the
[Toaster.DO](https://github.com/DECODEproject/toaster.do) project.

It can also export the Dockerfile to a JSON formatted AST.

```
usage: docker2sh.py [-h] [-j] [-s] [--keeptabs] Dockerfile

positional arguments:
  Dockerfile

optional arguments:
  -h, --help   show this help message and exit
  -j, --json   output the data as a JSON structure
  -s, --shell  output the data as a shell script (default)
  --keeptabs   do not replace \t (tabs) in the strings
```

# Licensing

Docker2sh is Copyright (C) 2018 - 2019 by the Dyne.org Foundation

Designed, written and maintained by Ivan J. and Denis Roio

This source code is free software; you can redistribute it and/or
modify it under the terms of the GNU Public License as published by
the Free Software Foundation; either version 3 of the License, or
(at your option) any later version.

This source code is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  Please refer
to the GNU Public License for more details.

You should have received a copy of the GNU Public License along with
this source code; if not, write to: Free Software Foundation, Inc.,
675 Mass Ave, Cambridge, MA 02139, USA.

