# Buscador de páginas web

Desarrollo incremental de un buscador que procesa páginas identificadas por su URL, título y relevancia. El contenido se normaliza antes de utilizarlo en las consultas.

## Evolución del proyecto

| Etapa | Qué incorpora |
|---|---|
| [001](001/README.md) | Lectura y enumeración de palabras |
| [002](002/README.md) | Normalización de mayúsculas y caracteres españoles |
| [003](003/README.md) | Intérprete de órdenes y lectura de páginas |
| [004](004/README.md) | Almacenamiento en una lista ordenada y consulta por URL |
| [200](200/README.md) | Tabla hash para almacenar y localizar páginas |
| [300](300/README.md) | Índice de palabras mediante un trie |

## Modelo de entrada

En las etapas con intérprete, la orden `i` introduce una página: relevancia, URL, título y contenido, que termina con la palabra `findepagina`. La orden `u` consulta una URL; `b` consulta una palabra en la etapa 300; `s` finaliza el programa.

## Estado de las búsquedas

En la etapa 300 funcionan las consultas por URL y palabra. Las órdenes `a`, `o` y `p`, previstas para búsquedas conjuntas, alternativas y por prefijo, siguen devolviendo cero resultados. En las etapas anteriores también hay operaciones todavía sin implementar.

La numeración corresponde a entregas académicas y permite seguir la evolución del código.
