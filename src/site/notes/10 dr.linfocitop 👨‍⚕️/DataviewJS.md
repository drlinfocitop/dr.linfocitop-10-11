---
{"dg-publish":true,"permalink":"/10-dr-linfocitop/dataview-js/","noteIcon":""}
---

#obsidian
## Primeros pasos
### ¡Hola mundo!
````
dv.paragraph("¡Hola mundo!")  
````
<p><span data-tag-name="p" class="el-p"><p>¡Hola mundo!</p></span></p>
### Uso del texto en DataviewJS
- En el operador ``dv.header(a,b)`` el primer elemento `a` de el orden del formato del encabezado para el texto siguiente que se representa como `b`.
````
dv.header(4, "Primeros pasos en DataviewJS")  
dv.paragraph('"Hola, *DataviewJS* resulta más eficiente que Dataview"')  
````
<h4><span data-tag-name="p" class="el-p"><p>Primeros pasos en DataviewJS</p></span></h4><p><span data-tag-name="p" class="el-p"><p>"Hola, <em>DataviewJS</em> resulta más eficiente que Dataview"</p></span></p>
### Listas explícitas en DataviewJS
````
dv.list(["Elemento 1", "Elemento 2", "Elemento 3"])  
````
<div><ul class="dataview list-view-ul"><li><span data-tag-name="p" class="el-p">Elemento 1</span></li><li><span data-tag-name="p" class="el-p">Elemento 2</span></li><li><span data-tag-name="p" class="el-p">Elemento 3</span></li></ul></div>
### Variables
````
const nombre = "Fernando"  
dv.paragraph("Hola, mi nombre es " + nombre + ".")
````
<p><span data-tag-name="p" class="el-p"><p>Hola, mi nombre es Fernando.</p></span></p>
- Otra variante es:
````
const nombre = "Fernando" 
dv.paragraph(`Hola, mi nombre es ${nombre}.`)
````
<p><span data-tag-name="p" class="el-p"><p>Hola, mi nombre es Fernando.</p></span></p>
## Listado en base a metadatos
- Ejemplo de ordenamiento de entradas en base a sus metadatos.
- Se muestra el código en Dataview y luego el correspondiente en DataviewJS:
````
LIST
FROM "21 Redes sociales 🔗"
WHERE web = youtube
````
- [[21 Redes sociales 🔗/Dudas Eternas\|Dudas Eternas]]
- [[21 Redes sociales 🔗/El Buen Librero\|El Buen Librero]]
- [[21 Redes sociales 🔗/Histeria del Perú\|Histeria del Perú]]
- [[21 Redes sociales 🔗/La Biblioteca de Merlín\|La Biblioteca de Merlín]]
- [[21 Redes sociales 🔗/La Peruanidad\|La Peruanidad]]

{ .block-language-dataview}
- Traducción a DataviewJS:
````
dv.list(dv.pages('"21 Redes sociales 🔗"')
.where(p =>p.web == "youtube").file.link)
````
<div><ul class="dataview list-view-ul"><li><span data-tag-name="p" class="el-p"><a data-tooltip-position="top" aria-label="21 Redes sociales 🔗/Dudas Eternas.md" data-href="21 Redes sociales 🔗/Dudas Eternas.md" href="21 Redes sociales 🔗/Dudas Eternas.md" class="internal-link" target="_blank" rel="noopener">Dudas Eternas</a></span></li><li><span data-tag-name="p" class="el-p"><a data-tooltip-position="top" aria-label="21 Redes sociales 🔗/El Buen Librero.md" data-href="21 Redes sociales 🔗/El Buen Librero.md" href="21 Redes sociales 🔗/El Buen Librero.md" class="internal-link" target="_blank" rel="noopener">El Buen Librero</a></span></li><li><span data-tag-name="p" class="el-p"><a data-tooltip-position="top" aria-label="21 Redes sociales 🔗/Histeria del Perú.md" data-href="21 Redes sociales 🔗/Histeria del Perú.md" href="21 Redes sociales 🔗/Histeria del Perú.md" class="internal-link" target="_blank" rel="noopener">Histeria del Perú</a></span></li><li><span data-tag-name="p" class="el-p"><a data-tooltip-position="top" aria-label="21 Redes sociales 🔗/La Biblioteca de Merlín.md" data-href="21 Redes sociales 🔗/La Biblioteca de Merlín.md" href="21 Redes sociales 🔗/La Biblioteca de Merlín.md" class="internal-link" target="_blank" rel="noopener">La Biblioteca de Merlín</a></span></li><li><span data-tag-name="p" class="el-p"><a data-tooltip-position="top" aria-label="21 Redes sociales 🔗/La Peruanidad.md" data-href="21 Redes sociales 🔗/La Peruanidad.md" href="21 Redes sociales 🔗/La Peruanidad.md" class="internal-link" target="_blank" rel="noopener">La Peruanidad</a></span></li></ul></div>
## Resumen de códigos JS
- `dv.pages(source)`
	- ``dv.pages()``: Todas la páginas del Vault 
	- ``dv.pages("#libros")``: Todas la entradas con el tag 'libros' 
	- ``dv.pages('"folder"')``: Todas las páginas del folder "folder" 
	- ``dv.pages("#si or -#no")``: Todas las páginas con el tag `#si`, o el que NO TIENE el tag `#no`
	- ``dv.pages('"folder" or #libros')``: Todas las páginas con el tag `#libros`, o con el folder "folder"
- `dv.list(elements)`
	- ``dv.list([1, 2, 3])``: lista de 1, 2, 3 
	- ``dv.list(dv.pages().file.name)``: Lista de todos los nombres
	- ``dv.list(dv.pages().file.link)``: Lista de todos los links
	- ``dv.list(dv.pages("#book").where(p => p.rating > 7))``: Lista de todos los libros con rating mayor que 7
## Lista de tareas
- `dv.taskList(tasks, groupByFile)`
	- `page.file.tasks`: Lista de vista de datos
	- `groupByFile`: si es verdadero, las tareas se agruparán automáticamente según el archivo del que provienen.
```
// List all tasks from pages marked '#project' dv.taskList(dv.pages("#project").file.tasks) 

// List all *uncompleted* tasks from pages marked #project dv.taskList(dv.pages("#project").file.tasks .where(t => !t.completed)) 

// List all tasks tagged with '#tag' from pages marked #project dv.taskList(dv.pages("#project").file.tasks .where(t => t.text.includes("#tag")))
```
## Tablas en DataviewJS
- `dv.table(headers, elements)`
	- `headers` son los encabezados de la tabla, expresados en forma de vector.
	- `elements` es la matriz de filas.
- Ejemplo para una tabla explícita:
```
dv.table( 
	["Col1", "Col2", "Col3"], 
		[ 
			["Row1", "Dummy", "Dummy"], 
			["Row2", 
				["Bullet1", "Bullet2", "Bullet3"], 
					"Dummy"], 
			["Row3", "Dummy", "Dummy"] 
		]
	 );
```
- Ejemplo práctico:
````
dv.table(["Influencers", "Red social"], 
	 dv.pages('"21 Redes sociales 🔗"')
		.where(b => b.influencer == true)
		.sort(b => b.web) 
		.map(b => [b.file.link, b.web]))
````
<div><table class="dataview table-view-table"><thead class="table-view-thead"><tr class="table-view-tr-header"><th class="table-view-th"><span data-tag-name="p" class="el-p">Influencers</span><span class="dataview small-text">5</span></th><th class="table-view-th"><span data-tag-name="p" class="el-p">Red social</span></th></tr></thead><tbody class="table-view-tbody"><tr><td><span data-tag-name="p" class="el-p"><a data-tooltip-position="top" aria-label="21 Redes sociales 🔗/Dudas Eternas.md" data-href="21 Redes sociales 🔗/Dudas Eternas.md" href="21 Redes sociales 🔗/Dudas Eternas.md" class="internal-link" target="_blank" rel="noopener">Dudas Eternas</a></span></td><td><span data-tag-name="p" class="el-p">youtube</span></td></tr><tr><td><span data-tag-name="p" class="el-p"><a data-tooltip-position="top" aria-label="21 Redes sociales 🔗/El Buen Librero.md" data-href="21 Redes sociales 🔗/El Buen Librero.md" href="21 Redes sociales 🔗/El Buen Librero.md" class="internal-link" target="_blank" rel="noopener">El Buen Librero</a></span></td><td><span data-tag-name="p" class="el-p">youtube</span></td></tr><tr><td><span data-tag-name="p" class="el-p"><a data-tooltip-position="top" aria-label="21 Redes sociales 🔗/Histeria del Perú.md" data-href="21 Redes sociales 🔗/Histeria del Perú.md" href="21 Redes sociales 🔗/Histeria del Perú.md" class="internal-link" target="_blank" rel="noopener">Histeria del Perú</a></span></td><td><span data-tag-name="p" class="el-p">youtube</span></td></tr><tr><td><span data-tag-name="p" class="el-p"><a data-tooltip-position="top" aria-label="21 Redes sociales 🔗/La Biblioteca de Merlín.md" data-href="21 Redes sociales 🔗/La Biblioteca de Merlín.md" href="21 Redes sociales 🔗/La Biblioteca de Merlín.md" class="internal-link" target="_blank" rel="noopener">La Biblioteca de Merlín</a></span></td><td><span data-tag-name="p" class="el-p">youtube</span></td></tr><tr><td><span data-tag-name="p" class="el-p"><a data-tooltip-position="top" aria-label="21 Redes sociales 🔗/La Peruanidad.md" data-href="21 Redes sociales 🔗/La Peruanidad.md" href="21 Redes sociales 🔗/La Peruanidad.md" class="internal-link" target="_blank" rel="noopener">La Peruanidad</a></span></td><td><span data-tag-name="p" class="el-p">youtube</span></td></tr></tbody></table></div>

>[!tips] Fuentes:
>- https://blacksmithgu.github.io/obsidian-dataview/api/code-reference/
>- https://medium.com/@biscotty666/a-gentle-introduction-to-dataviewjs-2eefcc59ee07
>- https://forum.obsidian.md/t/learning-dataviewjs-from-dataview/48056/6
>- https://momentjs.com/