
bash-envrc
==========

### Enhance GNU Bash with Environment Variable Run-Commands

About
-----

This is an elaborated [GNU Bash](https://www.gnu.org/software/bash/)
run-command script which enhances interactive shell sessions with the
possibility to automatically activate environment variables through
the execution of (explicitly to be whitelisted) `.envrc` run-command scripts.

Usage
-----

- `$ vi ~/.bash_login`:

    ```
    source /path/to/bash-envrc.rc
    envrc switch -i $HOME
    ```

- `$ vi ~/prj/foo/.bash_envrc`:

    ```
    -> echo "++ entering project \"foo\""
    <- echo "++ leaving project \"foo\""
    PATH! ^= ${PWD}/bin:
    ```

- `$ envrc add ~/prj/foo`

License
-------

Copyright (c) 2018-2019 Dr. Ralf S. Engelschall (http://engelschall.com/)

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

