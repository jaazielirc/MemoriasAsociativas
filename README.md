# Memorias Asociativas (M.A)

_Es un pequeño ejemplo gráfico de cómo funcionan las memorias asociativas en la IA, en el README.md se mencionará cómo es que funcionan. Este programa fue hecho para la asignatura de Sistemas Expertos de la carrera Ingeniería en Computación en el CU UAEM Zumpango_

## Comenzando 🚀

_Existen las memorias asociativas Alfa Beta (AB)_

_M.A heteroasociativas Alfa-Beta_
```
Algoritmo M.A AB tipo máximo
```
```
Algortimo M.A AB tipo mínimo
```
```
Algoritmo M.A AB combinadas
```

_M.A autoasociativas AB_
```
Algoritmo M.A AB tipo máximo
```
```
Algoritmo M.A AB tipo mínimo
```
```
Algoritmo M.A AB combinados
```

## Este código utiliza las Memorias Alfa-Beta bidireccionales

_Operaciones binarias Alfa y Beta: definiciones y propiedades_

```
Las M.A AB utilzan máximos y mínimos, y dos operaciones binarias originales Alfa y Beta

Para la definición de las operaciones binarias Alfa y Beta se deben especificar los conjuntos A y B, los cuales son:
    A={0,1}   y   B={0, 1, 2}


La operación 'alfa': A x A -> B se define como se muestra en la tabla:

    | X | Y |  alfa(x,y) |
    ----------------------
    | 0 | 0 |     1      |
    | 0 | 1 |     0      |
    | 1 | 0 |     2      |
    | 1 | 1 |     1      |


La operación 'beta': B x A -> A se define como se muestra en la tabla:

    | X | Y |  beta(x,y)  |
    -----------------------
    | 0 | 0 |     0       |
    | 0 | 1 |     0       |
    | 1 | 0 |     0       | 
    | 1 | 1 |     1       |
    | 2 | 0 |     1       |
    | 2 | 1 |     1       |


Los conjuntos A y B y las operaciones binarias 'alfa' y 'beta' junto con los operadores Min(mínimo) y Max(máximo) usuales conforman el sistema algebráico (A,B,alfa,beta,Min,Max) en el que están inmersas las M.A Alfa-Beta.

Se requiere la definición de cuatro operaciones matriciales, e las cuales se usarán 4 casos particulares.


Operacion: alfaMaximo: 'Pmxr Delta x Qrxn' = [Fij ^ alfa]
```
### Ejemplo
```
a) [ 111010010110 ] -> [X' x (X')^t] y resulta en:
    
    alfa | 1 1 1 0 1 0 0 1 0 1 1 0 |
    --------------------------------
      1  | 1 1 1 2 1 2 2 1 2 1 1 2 |
      1  | 1 1 1 2 1 2 2 1 2 1 1 2 |
      1  | 1 1 1 2 1 2 2 1 2 1 1 2 |
      0  | 0 0 0 1 0 1 1 0 1 0 0 1 |
      1  | 1 1 1 2 1 2 2 1 2 1 1 2 |
      0  | 0 0 0 1 0 1 1 0 1 0 0 1 |
      0  | 0 0 0 1 0 1 1 0 1 0 0 1 |
      1  | 1 1 1 2 1 2 2 1 2 1 1 2 |
      0  | 0 0 0 1 0 1 1 0 1 0 0 1 |
      1  | 1 1 1 2 1 2 2 1 2 1 1 2 |
      1  | 1 1 1 2 1 2 2 1 2 1 1 2 |
      0  | 0 0 0 1 0 1 1 0 1 0 0 1 |

En el programa se puede agregar ruido aditivo y sustractivo para ver el resultado de las memorias con dicho efecto.
```
## Pre-requisitos 📋
_> Necesitas un compilador de Java, puede ser un editor de código como Visual Studio Code, NetBeans o bien en consola por medio de la [Instalación](http://elclubdelautodidacta.es/wp/2013/03/instalacion-del-kit-de-desarrollo-java-jdk-en-windows/)_
_> Descargar o copiar el repositorio_

## Modo de ejecución ⚙️
_Ejecuta el archivo 'Memorias.java' sea con un IDE, editor de código (VSCODE) o línea de comandos, que en ese caso primero debes posicionarte en la carpeta de los archivos, compilar con el comando 'javac Memorias.java' y 'javac MemoriasAsociativas.java', después ejecutar con 'java Memorias' y listo, debe aparecer la interfaz gráfica._