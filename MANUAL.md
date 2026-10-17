# Topología — Manual

Arq. Roberto Dip

Cómo sacar el modelo de Topología y abrirlo en otros programas, sobre todo en SketchUp, y el
resto de lo que hay en los menús. En línea: https://robertodip.github.io/topologia/manual.html

## Llevar el modelo a SketchUp

SketchUp no deja escribir su formato propio (.skp, es cerrado), así que Topología exporta un
**.dae** (Collada): el formato de intercambio que SketchUp importa con las medidas puestas, en
milímetros y con la z hacia arriba.

### Paso 1 — Exportar desde Topología

1. Dejá la figura como la querés llevar (cuerpo, fuerzas, operaciones, tirones).
2. Abrí el menú **Archivo** (arriba a la izquierda). La parte de arriba es **Exportar modelo
   como**.
3. En **Lado mayor** poné cuánto querés que mida, en milímetros, el lado más largo de la
   figura (viene en 80 mm). Debajo se ven las medidas que va a tener.
4. En **Resolución** mirá cuántos triángulos dice que va a tener el archivo. Si pasa de
   100.000, elegí **Media** o **Baja**: SketchUp se pone muy lento con tantos.
5. Hacé clic en **SketchUp**. Se descarga un archivo con un nombre como
   `topologia-toro-80mm.dae` en la carpeta **Descargas**.

### Paso 2 — Importar en SketchUp

Hace falta SketchUp **de escritorio** (Pro, Studio o la versión para estudiantes) o SketchUp
Go. El SketchUp gratuito de la web no importa estos archivos: ver
[¿Qué SketchUp sirve?](#que-sketchup-sirve).

1. Abrí SketchUp. Conviene una plantilla en **milímetros** (por ejemplo, «Arquitectura —
   Milímetros») para leer las medidas en mm; el tamaño llega bien con cualquier plantilla.
2. Menú **Archivo → Importar** (File → Import).
3. Abajo a la derecha del cuadro, en el tipo de archivo, elegí **COLLADA (\*.dae)**. Si no, el
   archivo no aparece en la lista.
4. Buscá el archivo en **Descargas** y seleccionalo (un clic, todavía no lo abras).
5. Clic en **Opciones** (Options). Dejá tildadas las dos casillas, que ya vienen así:
   **Validar archivo COLLADA** y **Unir caras coplanarias** (esta junta los triángulos de las
   caras planas, como las de un cubo, en una sola cara). **Aceptar**.
6. Clic en **Abrir** (Windows) o **Importar** (Mac).
7. Si el modelo queda pegado al cursor, hacé clic donde lo quieras ubicar (por ejemplo, en el
   cruce de los ejes). Si no lo ves, usá **Zoom Extents** (Ctrl+Mayús+E en Windows,
   Cmd+Mayús+E en Mac): encuadra todo el modelo.

### Paso 3 — Dejarlo prolijo

- **Se ven las aristas de todos los triángulos:** seleccioná el modelo, clic derecho →
  **Suavizar/alisar aristas** (Soften/Smooth Edges) y mové el control hasta que desaparezcan
  las líneas de las partes curvas.
- **Comprobar la medida:** con la **Cinta métrica** (Tape Measure) medí el lado más largo:
  tiene que dar el «Lado mayor» que elegiste.
- **Los ejes coinciden:** en Topología y en SketchUp la **x** es roja, la **y** verde
  (profundidad) y la **z** azul (hacia arriba). Lo que acá se estira «en z», en SketchUp
  también está en z.
- **Va lento o pesa mucho:** volvé a exportar con resolución **Media** o **Baja**. La forma
  y la topología son las mismas, con menos triángulos.
- **La cinta de Möbius** y las superficies planas llegan como superficies sin espesor (no son
  sólidos). Es correcto: no encierran volumen.

### ¿Qué SketchUp sirve?

Relevado en octubre de 2026; Trimble cambia los planes seguido.

| Versión | Dónde corre | ¿Importa el .dae? | Costo |
|---|---|---|---|
| SketchUp Free | Web | **No**: solo importa .skp, .jpg y .png | Gratis |
| SketchUp Go | Web y iPad | Sí | Pago |
| SketchUp Pro / Studio | Escritorio | Sí (y también DXF y STL) | Pago |
| SketchUp Studio para estudiantes | Escritorio | Sí (es la Pro) | US$ 55 por año (precio oficial); preguntá si tu facultad tiene licencias |
| SketchUp for Schools | Web | Sí | Gratis, solo para escuelas primarias y secundarias |
| SketchUp Make 2017 | Escritorio | Sí | Ya **no se descarga** del sitio oficial |

**SketchUp Make 2017:** si ya lo tenés instalado, el .dae se importa igual que en el paso 2.
No lo bajes de sitios no oficiales: es una versión vieja, sin actualizaciones de seguridad, y
las copias sueltas pueden traer programas dañinos.

**Si solo tenés el SketchUp gratuito de la web**, no puede abrir ningún archivo exportado por
Topología. Para mirar, medir o seguir trabajando el modelo usá alguno de los
[programas gratuitos](#otros-programas-gratuitos).

## Otros programas gratuitos

Todos son gratis. Con estos programas conviene **STL** u **OBJ**; el .dae solo lo abren
algunos.

| Programa | Dónde corre | Qué archivo abrir | Para qué | Descarga |
|---|---|---|---|---|
| **Online 3D Viewer** | En el navegador, sin instalar (también en el celular) | STL, OBJ o .dae | Mirar y girar el modelo; también lo pasa a otros formatos | https://3dviewer.net |
| **Tinkercad** | En el navegador, con cuenta gratuita de Autodesk | STL u OBJ (hasta 25 MB) | Modelar encima con formas simples; preparar para imprimir | https://www.tinkercad.com |
| **Blender** | Windows, Mac y Linux | OBJ o STL | Renders, materiales, animación | https://www.blender.org/download/ |
| **FreeCAD** | Windows, Mac y Linux | STL u OBJ | Dibujo técnico y CAD; llega como malla | https://www.freecad.org/downloads.php |
| **MeshLab** | Windows, Mac y Linux | STL, OBJ o .dae | Revisar la malla, repararla, bajarle triángulos | https://www.meshlab.net |
| **PrusaSlicer** | Windows, Mac y Linux | STL | Impresión 3D | https://www.prusa3d.com/page/prusaslicer_424/ |
| **UltiMaker Cura** | Windows, Mac y Linux | STL | Impresión 3D | https://ultimaker.com/software/ultimaker-cura/ |
| **OrcaSlicer** | Windows, Mac y Linux | STL | Impresión 3D | https://github.com/SoftFever/OrcaSlicer/releases |

Detalles:

- **Tinkercad:** al importar, elegí **milímetros** (con pulgadas sale de otro tamaño). Si el
  archivo pasa de 25 MB, exportá en resolución Media o Baja.
- **Blender:** desde la versión 5 ya no abre .dae; usá OBJ (se pone de pie solo) o STL.
- **Online 3D Viewer:** arrastrá el archivo a la página. Se abre en tu navegador: el archivo no
  se sube a ningún lado.
- **Autodesk Fusion** (licencia gratuita de uso personal): ver [más abajo](#autodesk-fusion-uso-personal).

## Exportar: formatos y medidas

Menú **Archivo → Exportar modelo como**. Todos los archivos salen en **milímetros**: el lado más
largo del cuerpo mide lo que indique «Lado mayor», y el cuerpo queda centrado y apoyado en el
piso.

| Formato | Para qué | Cómo entra |
|---|---|---|
| **SketchUp** | SketchUp de escritorio y Go (no la versión web gratuita) | Es un archivo **.dae** (Collada). Ver [Llevar el modelo a SketchUp](#llevar-el-modelo-a-sketchup). |
| **STL** | Impresión 3D (PrusaSlicer, OrcaSlicer, Cura, Bambu Studio); Tinkercad; Autodesk Fusion | Al importar, elegir milímetros. No está disponible en la cinta de Möbius: una superficie sin espesor no se puede imprimir. |
| **OBJ** | Blender, Rhino, Cinema 4D, Tinkercad | Viene con Y hacia arriba, como es costumbre en OBJ; Blender lo pone de pie solo. |
| **DXF** | AutoCAD, SketchUp Pro | Cada triángulo es una cara 3D. Llega como malla, no como sólido. |

### Resolución

- **Completa**: la malla tal como se ve en pantalla.
- **Media** y **Baja**: vuelven a armar el cuerpo con menos triángulos y le aplican las mismas
  fuerzas; la forma y la topología son las mismas y el archivo pesa mucho menos.

El menú muestra cuántos triángulos va a tener el archivo. SketchUp se pone lento por encima de
los 100.000: para esos casos conviene la resolución media o baja.

### Autodesk Fusion (uso personal)

La licencia gratuita de uso personal importa **STL** y **OBJ**; el **.dae no** y el **DXF**
solo en 2D (el nuestro es 3D, no sirve). Conviene el **STL**:

- **Insertar → Insertar malla** (Insert → Insert Mesh) y elegir **milímetros** en el diálogo:
  así queda en tamaño real (ni el STL ni el OBJ guardan las unidades).
- El STL viene con z hacia arriba (como en esta aplicación y en SketchUp); el OBJ, con y hacia
  arriba. Si la pieza aparece acostada, se endereza en el mismo diálogo de Insertar malla.
- Llega como malla. Para convertirla en sólido (Malla → Convertir malla) exportar en
  resolución **media o baja**: Fusion no convierte bien mallas de decenas de miles de triángulos.

## Imagen de la vista e impresión

Menú **Archivo → Exportar imagen de la vista**. Solo la ventana de la vista (el plano o el volumen que
está en pantalla, con la red, la malla, el original y los ejes si están prendidos), nunca los
paneles:

- **PNG**: fondo transparente.
- **JPG**: fondo blanco.
- **Imprimir** (también Ctrl+P): imprime solo la vista sobre el blanco del papel, en hoja
  apaisada si la imagen es más ancha que alta.

Siempre con los colores del tema claro (para que las líneas se vean sobre blanco), hasta 3
veces la resolución de la pantalla (lado máximo 4096 px) y recortada al dibujo con un margen.

## Guardar y recuperar figuras

**Guardar** (en la cabecera) guarda la figura que está en pantalla con un nombre: el cuerpo base
con las operaciones, las fuerzas (con sus valores y su orden), los tirones y la posición de la
barra t. Es una foto: no guarda cómo se llegó a ella. Si el nombre ya existe, avisa y la
reemplaza.

**Recuperar** muestra la lista de figuras guardadas (la más nueva arriba) con el cuerpo y las
transformaciones de cada una. «Recuperar» la pone en pantalla; se puede volver atrás con
**Deshacer**. «✕» la borra (pide un segundo clic).

Las figuras quedan guardadas en el navegador de esa computadora: otro navegador u otra
computadora no las ven, y se pierden si se borran los datos de navegación del sitio. Guardar
un modelo para usarlo en otro programa es otra cosa: eso es **Exportar**.
