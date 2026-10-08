# Recorridos de grafos

Dos ejercicios en C++ que exploran grafos dirigidos mediante recorridos en anchura y en profundidad.

| Archivo | Problema | Estructuras utilizadas |
|---|---|---|
| `402.cpp` | Recorrer los vértices en anchura, incluyendo las componentes que queden sin visitar | Matriz de adyacencia, cola y marcas de visita |
| `403.cpp` | Buscar un recorrido desde el primer vértice hasta el último mediante DFS | Listas de adyacencia y exploración con retroceso |

El primer ejercicio identifica los vértices mediante letras. El segundo utiliza índices numéricos y muestra el recorrido encontrado o `INFINITO` cuando no alcanza el destino. El recorrido DFS no calcula necesariamente el camino más corto.

## Compilación

```bash
g++ -std=c++11 402.cpp -o bfs
g++ -std=c++11 403.cpp -o dfs
```

Ejecuta `./bfs` o `./dfs` y proporciona los casos por la entrada estándar. Cada ejercicio tiene su propio formato de entrada, definido en su función principal.

[Volver a AED1](../README.md)
