---
{"dg-publish":true,"permalink":"/10-dr-linfocitop/dataview/","noteIcon":""}
---

- Extensión de [[10 dr.linfocitop 👨‍⚕️/Markdown\|Markdown]] llamada "**Data-Driven Documents**" (Documentos Orientados a Datos) que permite la creación de tablas interactivas y dinámicas. Con **DataView**, puedes trabajar con conjuntos de datos y mostrarlos de manera estructurada y manipulable.
- Se necesitas tener instalada la extensión correspondiente en tu editor o plataforma de [[10 dr.linfocitop 👨‍⚕️/Markdown\|Markdown]]. 
- Dataview no distingue mayúsculas de minúsculas en su código. Excepto que este acompañado por comillas "".
- A continuación, algunos conceptos clave:

## Listado sencillo
- Listado de todos los fichero (carpeta raíz): 
````
LIST 
FROM ""
LIMIT 10 
````
- [[00 Home 🌐/Apariencia Obsidian\|Apariencia Obsidian]]
- [[00 Home 🌐/Datos Personales 👨‍💼\|Datos Personales 👨‍💼]]
- [[00 Home 🌐/Home\|Home]]
- [[00 Home 🌐/Plantillas/Plantilla autor\|Plantilla autor]]
- [[00 Home 🌐/Plantillas/Plantilla libro - otro idioma\|Plantilla libro - otro idioma]]
- [[00 Home 🌐/Plantillas/Plantilla libro repositorio legal\|Plantilla libro repositorio legal]]
- [[00 Home 🌐/Plantillas/Plantilla libro\|Plantilla libro]]
- [[00 Home 🌐/Trivia libro - autor\|Trivia libro - autor]]
- [[00 Home 🌐/📚 Antropología autores\|📚 Antropología autores]]
- [[00 Home 🌐/📚 Antropología libros activos\|📚 Antropología libros activos]]

{ .block-language-dataview}

- Listado de todos los ficheros de la carpeta y subcarpetas:
````
LIST 
FROM "00 Home 🌐"
LIMIT 10
````
- [[00 Home 🌐/Apariencia Obsidian\|Apariencia Obsidian]]
- [[00 Home 🌐/Datos Personales 👨‍💼\|Datos Personales 👨‍💼]]
- [[00 Home 🌐/Home\|Home]]
- [[00 Home 🌐/Plantillas/Plantilla autor\|Plantilla autor]]
- [[00 Home 🌐/Plantillas/Plantilla libro - otro idioma\|Plantilla libro - otro idioma]]
- [[00 Home 🌐/Plantillas/Plantilla libro repositorio legal\|Plantilla libro repositorio legal]]
- [[00 Home 🌐/Plantillas/Plantilla libro\|Plantilla libro]]
- [[00 Home 🌐/Trivia libro - autor\|Trivia libro - autor]]
- [[00 Home 🌐/📚 Antropología autores\|📚 Antropología autores]]
- [[00 Home 🌐/📚 Antropología libros activos\|📚 Antropología libros activos]]

{ .block-language-dataview}

- Listado de todos los ficheros de la subcarpeta:
````
LIST 
FROM "00 Home 🌐/Plantillas"
LIMIT 10 
````
- [[00 Home 🌐/Plantillas/Plantilla autor\|Plantilla autor]]
- [[00 Home 🌐/Plantillas/Plantilla libro - otro idioma\|Plantilla libro - otro idioma]]
- [[00 Home 🌐/Plantillas/Plantilla libro repositorio legal\|Plantilla libro repositorio legal]]
- [[00 Home 🌐/Plantillas/Plantilla libro\|Plantilla libro]]

{ .block-language-dataview}

- Listado de todos los ficheros que tengan como **tag**: #obsidian
````
LIST 
FROM #obsidian
LIMIT 10 
````
- [[10 dr.linfocitop 👨‍⚕️/Markdown\|Markdown]]
- [[10 dr.linfocitop 👨‍⚕️/DataviewJS\|DataviewJS]]
- [[10 dr.linfocitop 👨‍⚕️/Callouts\|Callouts]]
- [[10 dr.linfocitop 👨‍⚕️/Digital Garden\|Digital Garden]]
- [[10 dr.linfocitop 👨‍⚕️/Dataview\|Dataview]]

{ .block-language-dataview}

### Uso de operadores
- Ejemplo **OR**:  todos los ficheros que se encuentren en *"00 Home 🌐/Plantillas"* **o** tengan el tag #obsidian 
````
LIST 
FROM "00 Home 🌐/Plantillas" OR #obsidian
LIMIT 10 
````
- [[00 Home 🌐/Plantillas/Plantilla autor\|Plantilla autor]]
- [[00 Home 🌐/Plantillas/Plantilla libro - otro idioma\|Plantilla libro - otro idioma]]
- [[00 Home 🌐/Plantillas/Plantilla libro repositorio legal\|Plantilla libro repositorio legal]]
- [[00 Home 🌐/Plantillas/Plantilla libro\|Plantilla libro]]
- [[10 dr.linfocitop 👨‍⚕️/Markdown\|Markdown]]
- [[10 dr.linfocitop 👨‍⚕️/DataviewJS\|DataviewJS]]
- [[10 dr.linfocitop 👨‍⚕️/Callouts\|Callouts]]
- [[10 dr.linfocitop 👨‍⚕️/Digital Garden\|Digital Garden]]
- [[10 dr.linfocitop 👨‍⚕️/Dataview\|Dataview]]

{ .block-language-dataview}

- Ejemplo **AND**: todos los ficheros que tengan el tag #obsidian **y** se encuentren en *"21 Redes sociales 🔗"*
````
LIST 
FROM #obsidian AND "21 Redes sociales 🔗"
LIMIT 5
````

{ .block-language-dataview}

- Ejemplo **AND** u **NOT** = **!**: todos los ficheros que **no** tengan el tag #obsidian **y** se encuentren en *"21 Redes sociales 🔗"*
````
LIST
FROM !#obsidian AND "21 Redes sociales 🔗"
LIMIT 5
````
- [[21 Redes sociales 🔗/Dudas Eternas\|Dudas Eternas]]
- [[21 Redes sociales 🔗/El Buen Librero\|El Buen Librero]]
- [[21 Redes sociales 🔗/Histeria del Perú\|Histeria del Perú]]
- [[21 Redes sociales 🔗/La Biblioteca de Merlín\|La Biblioteca de Merlín]]
- [[21 Redes sociales 🔗/La Peruanidad\|La Peruanidad]]

{ .block-language-dataview}
