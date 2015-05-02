# Mozilla Download [![Build Status](https://travis-ci.org/erikvold/fx-download.svg?branch=master)](https://travis-ci.org/erikvold/fx-download)

Helper utility for downloading various mozilla products in various
release channels. Built on top of
[fx-get-url](https://github.com/erikvold/fx-get-url).

Handles operating system detection (win32, mac, linux-i686,
linux-x86_64) and extraction of files (.tar.bz2, .dmg).
Extraction is platform dependent a .dmg may not unpack on linux.

## Usage

``` js
var fxdownload = require('fx-download');

var options = {};

// download firefox
fxdownload('save/me', options, functon(err, path) {
  // path is the same as save targe
});
```


## CLI Usage

```sh
fx-download path/to/place/extracted/folder
```

## License

The MIT License (MIT)

Copyright (c) 2013 Sahaja James Lal

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
