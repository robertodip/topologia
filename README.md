# Topología

Arq. Roberto Dip

Una aplicación para ver, en 3D, qué cambia y qué no cuando un cuerpo se deforma como si
fuera de goma: estirar, torcer, doblar o inflar no cambian su topología; cortar o perforar,
sí. Al costado, un panel cuenta los vértices, aristas y caras, y muestra que esos números
no se mueven mientras el área y el volumen sí.

Es gratis para estudiar y enseñar (ver la licencia, más abajo).


## Cómo abrirla

**Opción 1 — En línea (recomendada).** Abrí este enlace en Edge o Chrome:

    https://robertodip.github.io/topologia/

No hay que instalar nada y **siempre está en la última versión**. Hace falta internet solo
para abrirla. Si alguna vez parece vieja, recargá la página.

**Opción 2 — En la computadora, sin internet.**

1. Descargá **Topologia.zip**:
   https://github.com/robertodip/topologia/releases/latest/download/Topologia.zip
2. En la carpeta Descargas, clic derecho sobre **Topologia.zip** → **Extraer todo…** →
   **Extraer**. (Si se abre el .zip con doble clic y se entra a index.html desde ahí, la
   aplicación no anda: primero hay que extraerlo.)
3. En la carpeta extraída, doble clic en **index.html**. Se abre en el navegador.

Si index.html se abre con otro programa: clic derecho → **Abrir con** → Microsoft Edge o
Google Chrome.

Anda en cualquier PC con Windows 10 u 11 con Edge (viene instalado) o Chrome. También en
Mac y Linux con un navegador actualizado.


## Cómo actualizar la copia de la computadora

La copia de la Opción 2 no se actualiza sola. Cuando haya una versión nueva:

1. Borrá la carpeta **Topologia** vieja (o, si preferís, extraé la nueva en el mismo lugar
   y, cuando Windows pregunte, elegí **Reemplazar los archivos en el destino**).
2. Descargá el **Topologia.zip** nuevo desde el mismo enlace de arriba y extraelo como la
   primera vez.
3. Si tenías un acceso directo a index.html, volvé a crearlo apuntando a la carpeta nueva.

Lo importante es que no queden dos copias: es fácil seguir abriendo la vieja sin darse cuenta.

Las **figuras guardadas** (botón Guardar) no se pierden al actualizar: quedan en el navegador,
no en la carpeta, así que la copia nueva las ve si la abrís con el mismo navegador. Eso sí,
la versión en línea y la copia de la computadora no comparten las figuras: cada una tiene las
suyas.


## Primeros pasos

- **Arriba, dos pestañas:** *Superficies* (hojas planas y la cinta de Möbius) y
  *Volúmenes* (cubo, prismas, cilindro, esfera, toroide).
- **Mover la vista:** con el mouse, arrastrar para girar, la rueda para acercar, el botón
  derecho para desplazar. En el celular o la tableta: un dedo gira, dos dedos acercan y
  desplazan.
- **Fuerzas** (panel de la izquierda): torsión, flexión, plegar, ahusado, estirar,
  esferizar, ondulación, abollar. Se activan con su casilla y se ajustan con los
  deslizadores.
- **La barra t** va de la forma original (0) a la deformada (1): muestra que el cambio es
  continuo. **Animar** la recorre sola.
- **✋ Tirar:** arrastrar una zona de la superficie con el mouse, como si fuera goma.
- **Ejemplos:** cubo y esfera, taza y rosquilla, cinta de Möbius, abanico y otros, listos
  para mirar.
- **Operaciones NO topológicas** (en rojo, solo en Volúmenes): perforar y cortar. Son las
  que sí cambian la topología; el panel avisa cuando eso pasa.
- **Deshacer / Rehacer** en la cabecera.
- **Guardar / Recuperar** en la cabecera: «Guardar» guarda la figura como está (el cuerpo con
  sus operaciones, fuerzas y tirones) con el nombre que elijas; «Recuperar» la vuelve a poner.
  Quedan guardadas en ese navegador y esa computadora (no viajan con el archivo).

## El panel de la derecha

- **No cambian (topología):** vértices V, aristas A, caras C, la característica de Euler
  χ = V − A + C, el género (cantidad de perforaciones), si es cerrada y si es orientable.
  Debajo dice a qué figura es **equivalente** el cuerpo: una esfera, un toro, un disco…
- **Cambian (geometría):** área y volumen, con el porcentaje respecto del original.
- La **×** de la esquina lo cierra para ver la figura entera; el botón **Topología y
  geometría**, en la misma esquina, lo vuelve a abrir.

## Llevar el modelo a SketchUp (paso a paso)

**1. Exportar desde Topología**

1. Dejá la figura como la querés llevar.
2. Abrí **Archivo** → **Exportar modelo como**.
3. En **Lado mayor** poné cuánto querés que mida el lado más largo, en milímetros (viene en 80).
4. En **Resolución**, si dice más de 100.000 triángulos, elegí **Media** o **Baja** (SketchUp
   se pone lento).
5. Clic en **SketchUp**. Se descarga un archivo **.dae** (por ejemplo
   `topologia-toro-80mm.dae`) en **Descargas**. Si lo exportaste desde el celular, pasalo a
   la computadora donde está SketchUp (por correo, Google Drive o cable).

**2. Importar en SketchUp** (de escritorio: Pro, Studio o la versión para estudiantes)

1. **Archivo → Importar** (File → Import).
2. Abajo a la derecha, en el tipo de archivo, elegí **COLLADA (\*.dae)**.
3. Seleccioná el archivo en **Descargas** y clic en **Opciones**: dejá tildadas
   **Validar archivo COLLADA** y **Unir caras coplanarias** (ya vienen así). **Aceptar**.
4. **Abrir** (Windows) o **Importar** (Mac). Si queda pegado al cursor, clic para ubicarlo; si
   no lo ves, **Zoom Extents** (Ctrl+Mayús+E).
5. Si se ven todos los triángulos: seleccionalo, clic derecho → **Suavizar/alisar aristas**
   (Soften/Smooth Edges).

Llega en milímetros y con los mismos ejes: x roja, y verde, z azul hacia arriba.

**Ojo: el SketchUp gratuito de la web no importa estos archivos** (solo abre .skp e
imágenes): para mirar o seguir trabajando el modelo, usá uno de los programas gratuitos de
abajo.

## Otros programas gratuitos

Para mirar o seguir trabajando el modelo sin SketchUp. Con estos conviene exportar **STL** u
**OBJ** (Archivo → Exportar modelo como):

- **Online 3D Viewer** — en el navegador, sin instalar, también en el celular (STL, OBJ o
  .dae): https://3dviewer.net
- **Tinkercad** — en el navegador, con cuenta gratuita (STL u OBJ; al importar elegí
  milímetros): https://www.tinkercad.com
- **Blender** — renders y animación (OBJ o STL): https://www.blender.org/download/
- **FreeCAD** — CAD (STL u OBJ): https://www.freecad.org/downloads.php
- **MeshLab** — revisar y aliviar la malla (STL, OBJ o .dae): https://www.meshlab.net
- **Impresión 3D** (STL): PrusaSlicer, UltiMaker Cura u OrcaSlicer.

## Manual

El paso a paso completo, con los detalles de cada formato y de cada programa, está en el **manual**:
desde la aplicación, **Ayuda → Manual de uso**, o en línea en
https://robertodip.github.io/topologia/manual.html (en la copia de la computadora, también
`manual.html` dentro de la carpeta).

## Imagen e impresión

Menú **Archivo → Exportar imagen de la vista**: guarda lo que se ve en la vista (sin los
paneles) como **PNG** con fondo transparente o **JPG** con fondo blanco. **Imprimir** (o Ctrl+P)
imprime solo la vista, sobre el blanco del papel: el fondo oscuro no se imprime. La imagen sale
con los colores claros, a más resolución que la pantalla y recortada al cuerpo.

La aplicación recuerda en el navegador lo último que estabas haciendo.


## Si algo no anda

- **Dice «Faltan archivos de la aplicación»:** se abrió desde adentro del .zip. Extraelo
  primero (paso 2 de arriba).
- **Dice «El navegador no puede dibujar en 3D»:** usá Edge o Chrome actualizados. En la
  configuración del navegador → Sistema, activá «Usar la aceleración de gráficos cuando esté
  disponible» y reinicialo.
- **Va lenta:** cerrá otras pestañas; en notebooks, conectá el cargador. Con perforar y
  cortar es normal que tarde un segundo en rehacer el cuerpo.


## Comentarios y errores

Para avisar de un error o sugerir algo, escribí a **tesserakit.app@gmail.com**. Desde la
aplicación: menú **Archivo → Comentarios y errores**, que abre el correo con una guía y los
datos del navegador ya cargados. Contá qué estabas haciendo, qué esperabas y qué pasó; una
captura de pantalla ayuda mucho.

Si tenés cuenta de GitHub, también podés abrir un aviso en
https://github.com/robertodip/topologia/issues


## Licencia

© 2026 Arq. Roberto Dip. Se puede usar gratis para estudiar, enseñar e investigar, y
compartir completa, sin cambios y sin cobrar. Los modelos que exportes son tuyos. No se
permite quitar el nombre del autor, distribuir versiones modificadas ni venderla. El texto
completo está en **LICENCIA.md**.
