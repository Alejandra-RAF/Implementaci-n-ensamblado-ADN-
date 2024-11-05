Este proyecto implementa un algoritmo para construir un grafo de De Bruijn a partir de fragmentos de ADN (k-mers), determinar si existe un camino o ciclo Euleriano, y reconstruir la secuencia original de ADN. 
El programa esta definido por 5 funciones:
  1.	build_de_bruijn_graph(kmers): toma como entrada una lista de k-mers y construye un grafo donde los nodos representan los prefijos y sufijos de los k-mers, y las aristas indican las transiciones entre ellos.
  2.	has_eulerian_path_or_cycle(graph): verifica si el grafo cumple las condiciones necesarias para tener un camino o ciclo Euleriano. Esto implica revisar los grados de entrada y salida de cada nodo. Imprimiendo por pantalla si el grafo no posee un camino o ciclo Euleriano las razones, como problemas de conectividad o errores en las secuencias de ADN, y sugerirá posibles correcciones.
  3.	find_eulerian_path(graph): encuentra y devuelve un camino Euleriano si existe.
  4.	reconstruct_sequence(path): utiliza el camino o ciclo Euleriano encontrado para reconstruir la secuencia original de ADN.
  5.	create_networkx_graph(graph): crea un grafo dirigido utilizando NetworkX para visualizar los k-mers y el camino o ciclo Euleriano encontrado.

Ejemplo de uso
  1.	Ejecuta el script en tu entorno de Python.
  2.	Ingresa los fragmentos de ADN (k-mers) separados por espacios. Cada fragmento debe tener exactamente 4 caracteres y contener solo los símbolos A, C, G y T. 

Ejemplos de entradas
Algunos ejemplos de entradas con los que se ha probado el programa son:
  1.	ACGT CGTG GTGA TGAC
  2.	AGTC GTCA TCAG CAGT AGTT GTTG
  3.	GACG GCTT TTAC ACTA TATG TGTG
  4.	AGTT GTTG TTGA TGAC GACG ACGA CGAA GAAC AACG
