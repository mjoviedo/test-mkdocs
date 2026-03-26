!!! abstract "Contenido"
    Cada lección comienza con un recuadro de "Contenido". Aquí se puntean los contenidos incluídos en la lección.


# Estructura

El curso se compone de *Módulos*, *Capítulos* y *Lecciones*. De esta forma:

``` mermaid
graph TD
    A{Módulo 1} --> B(Capítulo 1);
    B --> C[Lección 1];
    B --> D[Lección 2];
    B --> E[etc...];
    A --> F[Capítulo 2];       
    F --> G[Lección 1];
    F--> H[etc];
```

A ver si la seguimos

``` mermaid
graph TD
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```
