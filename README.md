# ocamlearlybird: make OCaml debugging less sucks

`ocamlearlybird` is a debug adapter purely written in OCaml. See [debug adapter protocol]("https://microsoft.github.io/debug-adapter-protocol") to get more information.

# Installation

`ocamlearlybird` can be installed with opam:

```
opam install earlybird
```

# Features

- [x] Auto discover sources heuristically
- [x] Line breakpoints and column breakpoints
- [x] Basic `next`, `step in`, `step out` and `continue` commands
- [x] Inspect stack frames, local variables, closure variables and global variables
- [ ] Function breakpoints
- [ ] Limited expression evaluation
- [ ] Conditional breakpoints
- [ ] Time travel

# Documentation

By default `ocamlearlybird` use `stdin` and `stdout` for debug adapter protocol. To launch `ocamlearlybird` as debug adapter in server mode:

```
ocamlearlybird --server --port=4711
```
