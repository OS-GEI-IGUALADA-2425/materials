# Introducció a la programació C

## Esquelet d'un progrma en C

### Arguments del programa

La funció `main` pot rebre dos arguments:

- `argc`: Número d'arguments passats al programa.
- `argv`: Matriu de punter a caràcters amb els arguments passats al programa.

```c
int main(int argc, char *argv[]) {
    // Codi del programa
    return 0;
}
```

Per exemple, si executem el programa `./programa arg1 arg2`, tindrem que `argc = 3` i `argv = {"./programa", "arg1", "arg2"}`. On `argv[0]` és el nom del programa.

> **Nota**: El valor de retorn de la funció `main` indica si el programa s'ha executat correctament. Per convenció, si el programa s'ha executat correctament, retornem 0 i si hi ha hagut algun error, retornem un valor diferent de 0, normalment (negatiu).

Per exempe:

```c
#include <stdio.h>

int
main(int argc, char **argv) {
    int i;
    for (i=0; i<argc; i++) {
        printf("%s\n", argv[i]);
    }
    return 0;
}
```

Aquest programa ens permet imprimir tots els arguments que li passem. Seria una versió simple de la comanda `echo` de Linux.

En Rust, la funció `main` no rep cap argument. Per tant, si volem accedir als arguments del programa, hem de fer servir la llibreria `std::env`.

```rust
use std::env;

fn main() {
    let args: Vec<String> = env::args().collect();
    for arg in args {
        println!("{}", arg);
    }
}
```
