# rbenv-default-gems

This rbenv plugin hooks into the `rbenv install` command to
automatically install gems every time you install a new version of
Ruby.

## Installation

Make sure you have the latest rbenv and ruby-build versions, then run:

    git clone https://github.com/rbenv/rbenv-default-gems.git $(rbenv root)/plugins/rbenv-default-gems

## Usage

rbenv-default-gems automatically installs the gems listed in the
`$(rbenv root)/default-gems` file every time you successfully install a new
version of Ruby with `rbenv install`.

Specify gems in `$(rbenv root)/default-gems` by name, one per line. You may
optionally specify a version string after the name, or `--pre` to
install a prerelease version. For example:

    bundler
    bcat ~>0.6
    rails --pre

Blank lines and lines beginning with a `#` are ignored.

## License

(The MIT License)

Copyright (c) 2013 Sam Stephenson

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
