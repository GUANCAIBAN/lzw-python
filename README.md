# lzw-python
A minimalistic [LZW](https://en.wikipedia.org/wiki/Lempel%E2%80%93Ziv%E2%80%93Welch) implementation in Python 3, compatible with Unix [compress](https://en.wikipedia.org/wiki/Compress) program (typically **.Z** extension).

## Usage

```
$ python3 lzw.py --help
usage: lzw.py [-h] [-d] [-o OUTPUT] INPUT

LZW Compress/Decompress

positional arguments:
  INPUT                 Input file

optional arguments:
  -h, --help            show this help message and exit
  -d, --decompress      Decompress mode
  -o OUTPUT, --output OUTPUT
                        Output file
```

## Test

```
$ python3 lzw.py -o test/output.txt.Z test/Lorem_Ipsum.txt
$ sudo apt install ncompress
$ compress -d test/output.txt.Z
```

## License

Copyright (c) 2014-2019 P. Asimakopoulos

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <https://www.gnu.org/licenses/>.
