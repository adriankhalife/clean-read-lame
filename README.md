# LAME 3.100 as used in Clean Read

Clean Read (an audio editor for iPhone by Khalife Voice LLC) exports MP3 with **LAME 3.100**, the MP3 encoder by the LAME project (https://lame.sourceforge.io).

LAME is licensed under the GNU Library General Public License, version 2 or (at your option) any later version. Clean Read uses it under the **GNU Lesser General Public License, version 2.1**. LAME is included **unmodified** and is built as a **separate dynamic library**, apart from the app.

## What's here

`LAME-3.100-for-Clean-Read.tar.gz` holds the exact source used to build the LAME library inside Clean Read:

- `Sources/LAME/`: the encoder library (libmp3lame) from the official `lame-3.100.tar.gz` release (SHA-256 `ddfe36cab873794038ae2c1210557ad34857a4b6bdc515785d1da9e175b1da1e`), unmodified. Only the encoder files are included; the command-line front end and the decoder are not used.
- `Sources/LAME/config.h`: a build configuration file written for this build (it is not part of LAME's code).
- `Package.swift`: how the library is built (a Swift package producing a dynamic library).
- `COPYING`, `LICENSE`: LAME's license files.

## License

LAME is free software; you can redistribute it and/or modify it under the terms of the GNU Lesser General Public License as published by the Free Software Foundation; either version 2.1 of the License, or (at your option) any later version. It is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY. See `COPYING` in the archive and https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html.

This repository contains only LAME. The code of Clean Read itself is not here.
