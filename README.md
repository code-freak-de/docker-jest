jest Docker image
===================

[jest](https://jestjs.io/) as standalone Docker image.

The image is based on `node:10-alpine`. The version identifier refers the
jest version (e.g. `code-freak/jest:23.6.0` uses jest v23.6.0).

# Usage
Following the offical [Getting Started Guide](https://jestjs.io/docs/en/getting-started.html)
from jest (if you do not have any code written, yet). Please make sure your
project at least contains a `package.json` or `jest.config.js` file.

Afterwards you can test your code with docker:
```console
$ docker run --rm -t -v $(pwd):/code --workdir /code cfreak/jest:latest jest
```

You can try this inside the `example` directory which contains a simple
add function including a test.

# License
Copyright (C) 2018 Code FREAK

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
