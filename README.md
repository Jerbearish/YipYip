# Appa

Appa is an esolang inspired by [Ook!](https://esolangs.org/wiki/Ook!). Like its inspiration, Appa is
intended to be writeable by someone other than humans; in this case, it is meant for use by a
certain loveable [Avatar: The Last Airbender Character](https://avatar.fandom.com/wiki/Appa).

The repository contains several files related to the generation and running of Appa code. Please
see the short descriptions of each below.

Appa is in no way associated with or funded by Nickelodean or any other company. This is purely for
intended for fun and as an ode to a beloved companion.

## [`convert_to_appa.py`](convert_to_appa.py)

The `convert_to_appa.py` file serves the purpose of generating Appa code. It is a simple
translator for code from [Brainf*ck](https://en.wikipedia.org/wiki/Brainfuck) to Appa. It can be
called as follows:

```text
usage: convert_to_appa.py [-h] [--output OUTPUT] input

positional arguments:
  input                 the input file to convert

optional arguments:
  -h, --help            show this help message and exit
  --output OUTPUT, -o OUTPUT
                        the output file to write to
```

## [`appa.py`](appa.py)

The `appa.py` file serves as an interpreter for Appa code. It was adapted from Elliot Chance's guide
*Write Your Own Brainf*ck Interpreter*, which can be found
[here](https://levelup.gitconnected.com/write-your-own-brainfuck-interpreter-98e828c72854).

It can be called as follows:

```text
usage: appa.py [-h] [--save-generated] input

positional arguments:
  input                 the input Appa file to run

optional arguments:
  -h, --help            show this help message and exit
  --save-generated, -s  save the generated lex and yacc files
```

## [`examples`](examples/README.md)

The `examples` directory includes example files related to the Appa language and translating to it.

## Contributing & Issues

This is an ongoing project; it does not have a full set of Turing operations, as the input delimeter
is currently ignored. There are other areas for improvement. Please feel free to open any Issues or
Pull Requests against the repository. Thanks in advance!
