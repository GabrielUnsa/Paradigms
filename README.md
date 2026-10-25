# Paradigms — Paradigmas de programación

Ejercicios académicos de programación funcional con Haskell, lógica con Prolog y orientada a objetos con Python. El repositorio incluye funciones sobre listas y números, bases de conocimiento, recorridos de grafos, ejemplos de clases y trabajos de equipo sobre matrices ralas y cifrado César.

Estos ejercicios prácticos fueron realizados durante el cursado de diversas materias mientras estudiaba la **Licenciatura en Análisis de Sistemas (Plan 2010)** de la **Universidad Nacional de Salta**.

**Materia:** ______________________________

## Contenido

- [Estructura](#estructura)
- [Haskell: programación funcional](#haskell-programación-funcional)
- [Prolog: programación lógica](#prolog-programación-lógica)
- [Python: orientación a objetos](#python-orientación-a-objetos)
- [Trabajos del equipo 3](#trabajos-del-equipo-3)
- [Preparación y ejemplos de uso](#preparación-y-ejemplos-de-uso)
- [Estado y compatibilidad](#estado-y-compatibilidad)
- [Licencia](#licencia)

## Estructura

```text
.
├── Haskell/
│   └── fun1.hs
├── Prolog/
│   ├── Grafo.pl
│   ├── Prolog.pl
│   ├── baseconoc.pl
│   ├── database.pl
│   └── ejemplo.pl
├── Python/
│   └── POO with Python/
│       ├── EjemploPOO.py
│       ├── EjemploPOO2.py
│       ├── EjemploPOO3.py
│       ├── EjemploPOO4.py
│       └── Herencia.py
├── Team 3 - Exercises/
│   ├── Haskell/fun1.hs
│   ├── Prolog/database.pl
│   └── Python/
│       ├── Cesar Encoding - Python/
│       └── TP3 - Python/
├── LICENSE
└── README.md
```

## Haskell: programación funcional

[Haskell/fun1.hs](Haskell/fun1.hs) reúne funciones independientes para experimentar desde GHCi.

| Tema | Ejemplos incluidos |
| --- | --- |
| Recursión numérica | Factorial (`fact1`), potencia (`pot`), producto mediante sumas, máximo común divisor (`euclides`) y mínimo común múltiplo (`mcm`). |
| Listas | Concatenación, producto de elementos, producto escalar, filtrado, inversión, incrementos y suma con `foldr`. |
| Teoría de números | Divisores, números perfectos, prueba de primalidad y generación de primos. |
| Cadenas y dígitos | Palíndromos, repetición de cadenas, inversión de enteros y extracción de dígitos. |
| Algoritmos y funciones de orden superior | Quicksort (`qsort`), búsqueda secuencial (`busSec`), evaluación de polinomios con Horner, `map` y aplicación repetida de funciones. |

Son definiciones para cargar en el intérprete; el archivo no contiene un programa `main` para ejecutarlo como aplicación de consola.

## Prolog: programación lógica

| Archivo | Contenido |
| --- | --- |
| [Prolog.pl](Prolog/Prolog.pl) | Hechos de parentesco y reglas para consultar abuelos y bisabuelos. |
| [Grafo.pl](Prolog/Grafo.pl) | Grafo dirigido con costos; consulta de aristas, trayectos de dos enlaces y caminos recursivos. |
| [baseconoc.pl](Prolog/baseconoc.pl) | Base mínima de hechos del predicado `esHombre/1`. |
| [database.pl](Prolog/database.pl) | Ejercicios de parentesco, palíndromos, suma y longitud de listas, reglas sobre plantas, clasificación de incendios, sensores y cursos. |
| [ejemplo.pl](Prolog/ejemplo.pl) | Borrador de hechos y reglas sobre riqueza y felicidad; contiene variables en hechos y referencias a predicados no definidos en ese archivo. |

Las reglas de plantas e incendios son ejercicios de representación de conocimiento. Los archivos contienen predicados de distintos ejercicios y conviene cargarlos por separado para evitar mezclar definiciones.

## Python: orientación a objetos

La carpeta [POO with Python](Python/POO%20with%20Python/) contiene los siguientes ejemplos:

| Archivo | Tema y comportamiento |
| --- | --- |
| `EjemploPOO.py` | Clase de televisores, atributos, encendido y apagado. Conserva un ejemplo de gelatinas comentado. Define `main()` sin invocarla automáticamente. |
| `EjemploPOO2.py` | Herencia simple y múltiple mediante electrodomésticos, teléfonos, celulares y televisores. Define `main()` sin invocarla. |
| `EjemploPOO3.py` | Encapsulamiento mediante atributos con doble guion bajo y métodos de consulta. Define `main()` sin invocarla. |
| `EjemploPOO4.py` | Lista enlazada de nombres y edades con menú de inserción, consulta y eliminación. El menú se ejecuta al cargar el archivo. |
| `Herencia.py` | Herencia entre `CasaStark` y `HerederoStar`. La demostración está en `main()` y se puede invocar con Python 3. |

Los cuatro archivos `EjemploPOO*.py` conservan sintaxis de Python 2, como `print` sin paréntesis y, en algunos casos, `raw_input`. Requieren ese intérprete o una adaptación a Python 3.

## Trabajos del equipo 3

| Carpeta | Proyecto |
| --- | --- |
| [Haskell](Team%203%20-%20Exercises/Haskell/) | Variante de `fun1.hs` con las funciones de estudio y un intento adicional de búsqueda binaria. |
| [Prolog](Team%203%20-%20Exercises/Prolog/) | Otra versión de la base de conocimiento `database.pl`, con ejercicios de reglas y listas. |
| [Cesar Encoding - Python](Team%203%20-%20Exercises/Python/Cesar%20Encoding%20-%20Python/) | Clases `Archivo` y `Cesar`, menú de archivos, cifrado y descifrado por desplazamiento, e intento de inferir la clave mediante `words.txt`. El alfabeto incluye letras minúsculas, punto, coma y espacio. |
| [TP3 - Python](Team%203%20-%20Exercises/Python/TP3%20-%20Python/) | `Ejercicio12.py` y `Ejercicio12P.py`: representación de matrices ralas mediante diccionarios de coordenadas, carga de dos matrices, visualización, suma y comparación. |

Estos trabajos de Python también corresponden a Python 2 y conservan partes incompletas. El menú de César importa `ClsCesar2`, pero solo se incluye `ClsCesar.py`. En `ClsFile.py`, la segunda definición de `Escribe` sustituye a la primera. Por ello, el menú necesita correcciones antes de utilizarse. `words.txt` debe estar disponible en el directorio de trabajo para el intento de descifrado sin clave.

## Preparación y ejemplos de uso

Los comandos de terminal usan Bash y parten de la raíz del repositorio:

```bash
git clone https://github.com/GabrielUnsa/Paradigms.git
cd Paradigms
```

Cada lenguaje se utiliza por separado: GHC/GHCi para Haskell, un intérprete como SWI-Prolog para Prolog y el intérprete de Python correspondiente al ejemplo.

### Haskell

```bash
ghci Haskell/fun1.hs
```

Dentro de GHCi se pueden evaluar:

```haskell
fact1 5
qsort [3, 1, 2, 1]
palindromo "reconocer"
```

Los resultados esperados de estas funciones son `120`, `[1,1,2,3]` y `True`, respectivamente. Para salir de GHCi, usar `:quit`.

### Prolog

```bash
swipl -s Prolog/Prolog.pl
```

En el intérprete:

```prolog
?- abuelo(clara, jose).
?- bisabuelo(ana, jose).
```

Ambas consultas se deducen como verdaderas a partir de los hechos incluidos. Para explorar el grafo en otra sesión:

```bash
swipl -s Prolog/Grafo.pl
```

```prolog
?- llegar(b, f, Intermedio, Costo).
```

El trayecto de dos enlaces pasa por `h` y tiene costo `13`. Para salir de SWI-Prolog, usar `halt.`.

### Python

Para ejecutar la demostración de herencia con Python 3 e invocar explícitamente su función principal:

```bash
python3 -c "import runpy; runpy.run_path('Python/POO with Python/Herencia.py')['main']()"
```

En un entorno que ya disponga de Python 2, un ejemplo histórico se puede cargar e invocar así:

```bash
cd "Python/POO with Python"
python2 -c "import EjemploPOO2; EjemploPOO2.main()"
```

## Estado y compatibilidad

Se ejecutó la demostración `Herencia.py` con Python 3.13.5. Además de los mensajes, imprime `None` porque `main()` muestra el valor devuelto por métodos que no retornan un resultado. No se ejecutaron los ejemplos de Python 2, Haskell o Prolog: esos intérpretes no estaban disponibles en el entorno de documentación.

El material conserva errores y casos pendientes de ejercicios:

- En ambos archivos Haskell, `xor` está definida mediante `&&`; su comportamiento corresponde a una conjunción. Algunas funciones también carecen de casos para listas de un elemento, listas de distintas longitudes o entradas negativas.
- La búsqueda binaria de la versión Haskell del equipo utiliza nombres no definidos (`lista` y `lenght`) y requiere corregirse antes de cargar esa versión completa.
- El grafo de Prolog contiene ciclos y `camino/2` no mantiene una lista de visitados, por lo que ciertas consultas pueden no terminar.
- Los ejercicios de matrices conservan nombres de atributos inconsistentes y fragmentos que requieren revisión de indentación y lógica antes de ejecutarlos.
- Los trabajos de Python utilizan `os.system("cls")`, que corresponde a la consola de Windows.

No hay un sistema de ejecución común ni pruebas automatizadas incluidas. Las versiones del directorio principal y las del equipo deben estudiarse como alternativas, sin combinarlas automáticamente.

## Licencia

Distribuido bajo la [licencia MIT](LICENSE). Copyright © 2025 Gabriel Marmanillo.
