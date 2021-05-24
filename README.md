# IMPLEMENTACI-N-DEL-ALGORITMO-A-
RESOLUCIÓN DE PROBLEMA MEDIANTE  BÚSQUEDA HEURÍSTICA

RESOLUCIÓN DE PROBLEMA MEDIANTE BÚSQUEDA HEURÍSTICA

IMPLEMENTACIÓN DEL ALGORITMO A*

Se tiene que implementar un algoritmo de A* cuyas funciones consistirán en que un robot se desplace desde una posición inicial (meta) hasta donde se encuentra un repositorio (destino), cargar este repositorio y llevarlo a unas posiciones predeterminadas.
En el ejercicio que se plantea se tienen tres repositorios y el robot tendrá que trasportarlos desde donde se encuentran a los puntos que se indican. Para ello las consideraciones que se hacen serán las siguiente:

Para ello las consideraciones que se hacen serán las siguiente teniendo en cuenta que hay que hacer tres viajes.

  1. Hay que decidir cuál será el primer viaje, el segundo y el tercero, para ello se calculará la h* de ida y vuelta y se empezará por la que menor coste tenga, después se recalculará para ver cuál de las otras  dos tiene menor h* desde la nueva posición del robot para decidir qué acción se ejecuta en segundo  lugar.

  2. Se considera que los repositorios no se pueden atravesar, es decir que los repositorios que no se muevan son considerados obstáculos cuando el robot esté transportando otro, y si se considera que  el robot cuando se desplaza solo, puede pasar por debajo de los repositorios.
  
  3. Habrá dos mapas, el original donde se reflejarán todo en cadena de caracteres y otro numérico para poder hacer mejor todas las consideraciones pertinentes.
  
A continuación, se muestra la disposición del mapa, indicando donde está el repositorio 1 (M1), el repositorio 2 (M2), el repositorio 3 (M3) y el robot (R). Las almohadillas (#) son considerados obstáculos  que el robot no puede atravesar.

En el mapa numérico se traducirá todo esto como, M1=5, M2=4, M3=3, R=2, #=1 y los espacios vacíos que no son obstáculos como un 0.
