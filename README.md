# dokku-shoreman

dokku-shoreman is a plugin for [dokku][dokku] that injects a stripped down
version of [shoreman][shoreman], a Procfile runner written in bash.

Normally, dokku only runs the `web` process within Procfile. The dokku-shoreman
plugin will run all process types (web, worker, etc.) and stop them all together.

## Installation

```sh
git clone https://github.com/statianzo/dokku-shoreman.git /var/lib/dokku/plugins/dokku-shoreman
dokku plugins-install
```

All future deployments will use shoreman to start all processes.

## License

The MIT License (MIT)

Copyright (c) 2013 Jason Staten

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
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[dokku]: https://github.com/progrium/dokku
[shoreman]: https://github.com/hecticjeff/shoreman
