# Pure OCaml SHA1
An implementation of the SHA1 hash function in pure OCaml, with no dependencies
except `ocamlc`. The main interesting function is
```ocaml
val digest : bytes -> bytes
```
which produces a SHA1 digest.

Not rigorously tested or recommended for production use, especially since a SHA1
collision has now been found. I mostly wrote this because I could not find a
pure OCaml implementation for the [Cryptopals
challenges](https://cryptopals.com/). 

To test it, *uncomment the end of `sha1.ml`* and run:
```bash
make
./sha1 "test-string"
```

