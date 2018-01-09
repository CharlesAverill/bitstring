# OCaml Bistring Library

```
Copyright (C) 2008-2016 Red Hat Inc, Richard W.M. Jones.
Copyright (C) 2016-2018 Red Hat Inc, Richard W.M. Jones, Xavier R. Guerin.
```

The original `README` content can be found in the `README.orig` file.

## Documentation

The documentation is located [here](http://xguer.in/bitstring).

## How to install

`opam install bitstring`

## How to use

### Ocamlfind

```
ocamlfind c -package bitstring -package bitstring.ppx -linkpkg ...
```

### Jbuilder

```lisp
(jbuild_version 1)

(executable
 ((name        foo)
  (libraries   (bitstring))
  (preprocess  (pps (bitstring.ppx)))
  ))
```

## How to build

`bitstring` version `3` requires OCaml `>= 4.06.0`.

### Dependencies

* `str`
* `unix`
* `compiler-libs`
* `ppx_tools_versioned`
* `ocaml-migrate-parsetree`

### Building the project

```
$ jbuilder build
```

### Running the tests

```
$ jbuilder runtest
```

## License

The library is licensed under the LGPL v2 or later, with the OCaml linking
exception. See the file COPYING.LIB for full terms. Programs are licensed under
the gpl v2 or later. see the file copying for full terms. All examples and tests
are public domain.
