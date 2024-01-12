---
{"dg-publish":true,"permalink":"/10-dr-linfocitop/callouts/","noteIcon":""}
---

#obsidian
+ Use `callouts` para incluir contenido adicional sin interrumpir el flujo de sus notas.
+ Para crear una llamada, agregue `[!info]` a la primera línea de una cita en bloque, donde `info` está el identificador de tipo . El identificador de tipo determina cómo se ve y se siente la llamada.


```
> [!info]
> Aquí hay un callout.
> Es compatible con **Markdown**, [[Internal link\|Wikilinks]] y [[Embed files\|embeds]]!
> ![cover_M.png|200](/img/user/02%20Image/cover_M.png)
```


> [!info]
> Aquí hay un callout.
> Es compatible con **Markdown**, [[Internal link|Wikilinks]] y [[Embed files|embeds]]!
> ![cover_M.png|200](/img/user/02%20Image/cover_M.png)

+ Las llamadas también se admiten de forma nativa en Obsidian Publish .
>[!note]
>Si también está utilizando el complemento Admonitions, debe actualizarlo al menos a la versión 8.0.0 para evitar problemas con la nueva función de llamada.

## Cambiar el titulo
+ De forma predeterminada, el título de la llamada es su identificador de tipo en mayúsculas y minúsculas. Puede cambiarlo agregando texto después del identificador de tipo:

```
> [!tip] Las llamadas pueden tener títulos personalizados
> Como éste.
```
> [!tip] Las llamadas pueden tener títulos personalizados
> Como éste.

+ Incluso puede omitir el cuerpo para crear llamadas de solo título:

```
> [!tip] Title-only callout
```
> [!tip] Title-only callout
## Callouts plegables
+ Puede hacer que una llamada sea plegable agregando un signo más (+) o un signo menos (-) directamente después del identificador de tipo.
+ Un signo más expande la llamada de forma predeterminada y un signo menos la contrae.

> [!faq]- ¿Los textos destacados son plegables?
> Sí! En una llamada plegable, el contenido se oculta cuando la llamada está contraída.

## Textos destacados anidados
+ Puede anidar llamadas en varios niveles.

```
> [!question] Can callouts be nested?
> > [!todo] Yes!, they can.
> > > [!example]  You can even use multiple layers of nesting.
```
> [!question] Can callouts be nested?
> > [!todo] Yes!, they can.
> > > [!example]  You can even use multiple layers of nesting.

## Estilos
+ Es posible mejorar el estilo con CSS.
+ A menos que  , cualquier tipo no compatible tiene como valor predeterminado el tipo `note`. 
+ El identificador de tipo no distingue entre mayúsculas y minúsculas.
### note
```
> [!note]
> Lorem ipsum dolor sit amet
```
> [!note]
> Lorem ipsum dolor sit amet

### abstract, sumary, tldr
```
> [!abstract]
> Lorem ipsum dolor sit amet
```
> [!abstract]
> Lorem ipsum dolor sit amet

### info

```
> [!info]
> Lorem ipsum dolor sit amet
```
> [!info]
> Lorem ipsum dolor sit amet
### todo

```
> [!todo]
> Lorem ipsum dolor sit amet
```
> [!todo]
> Lorem ipsum dolor sit amet
### tip

```
> [!tip]
> Lorem ipsum dolor sit amet
```
> [!tip]
> Lorem ipsum dolor sit amet
### success, check, done

```
> [!success]
> Lorem ipsum dolor sit amet
```
> [!success]
> Lorem ipsum dolor sit amet
### question, help, faq

```
> [!question]
> Lorem ipsum dolor sit amet
```
> [!question]
> Lorem ipsum dolor sit amet
### warning, caution, attention

```
> [!warning]
> Lorem ipsum dolor sit amet
```
> [!warning]
> Lorem ipsum dolor sit amet
### failure, fail, missing

```
> [!failure]
> Lorem ipsum dolor sit amet
```
> [!failure]
> Lorem ipsum dolor sit amet
### danger, error

```
> [!danger]
> Lorem ipsum dolor sit amet
```
> [!danger]
> Lorem ipsum dolor sit amet
### bug

```
> [!bug]
> Lorem ipsum dolor sit amet
```
> [!bug]
> Lorem ipsum dolor sit amet
### example

```
> [!example]
> Lorem ipsum dolor sit amet
```
> [!example]
> Lorem ipsum dolor sit amet
### quote, cite

```
> [!quote]
> Lorem ipsum dolor sit amet
```
> [!quote]
> Lorem ipsum dolor sit amet



>[!tips] Fuentes:
>- https://blacksmithgu.github.io/obsidian-dataview/api/code-reference/
>- https://medium.com/@biscotty666/a-gentle-introduction-to-dataviewjs-2eefcc59ee07
>- https://forum.obsidian.md/t/learning-dataviewjs-from-dataview/48056/6
>- https://momentjs.com/