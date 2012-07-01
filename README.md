canvas-grafocondorcet
=====================

La función grafo_condorcet es una utilidad escrita en javascript que dibuja el grafo dirigido asociado a la matriz de pares del método de votación preferencial Condorcet-Schulze en un canvas. No depende de ningún framework y funciona en cualquier navegador que soporte HTML5

Puedes encontrar una explicación completa del método en http://en.wikipedia.org/wiki/Schulze_method

USO
---

1. Incluir grafocondorcet.js en el head de tu página:

`<script src="grafocondorcet.js" type="text/javascript"></script>`

2. Definir la etiqueta o etiquetas canvas dentro del body y darle un nombre al atributo id:

`<canvas id="grafo" width="600" height="600"><canvas>`

3. Invocar la función:

<code>
	<script type="text/javascript">
		var votaciones = [
			["A", 0, 20, 26, 30, 22],
			["B", 25, 0, 16, 33, 18],
			["C", 19, 29, 0, 17, 24],
			["D", 15, 12, 28, 0, 14],
			["E", 23, 27, 21, 31, 0]
			];
	
		var canvas = grafo_condorcet ('grafo', votaciones);
	</script>
</code>

LICENCIA
--------
GPL
