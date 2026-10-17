# Topología — Manual

Arq. Roberto Dip

## Guardar y recuperar figuras

**Guardar** (en la cabecera) guarda la figura que está en pantalla con un nombre: el cuerpo base
con las operaciones, las fuerzas (con sus valores y su orden), los tirones y la posición de la
barra t. Es una foto: no guarda cómo se llegó a ella. Si el nombre ya existe, avisa y la
reemplaza.

**Recuperar** muestra la lista de figuras guardadas (la más nueva arriba) con el cuerpo y las
transformaciones de cada una. «Recuperar» la pone en pantalla; se puede volver atrás con
**Deshacer**. «✕» la borra (pide un segundo clic).

Las figuras quedan guardadas en el navegador de esa computadora: otro navegador u otra
computadora no las ven, y se pierden si se borran los datos de navegación del sitio.

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

## Exportar

Menú **Archivo → Exportar modelo como**. Todos los archivos salen en **milímetros**: el lado más
largo del cuerpo mide lo que indique «Lado mayor», y el cuerpo queda centrado y apoyado en el
piso.

| Formato | Para qué | Cómo entra |
|---|---|---|
| **STL** | Impresión 3D (PrusaSlicer, OrcaSlicer, Cura, Bambu Studio); Autodesk Fusion | Al importar, elegir milímetros. No está disponible en la cinta de Möbius: una superficie sin espesor no se puede imprimir. |
| **OBJ** | Blender, Rhino, Cinema 4D | Viene con Y hacia arriba, como es costumbre en OBJ; Blender lo pone de pie solo. |
| **DXF** | AutoCAD, SketchUp Pro, FreeCAD | Cada triángulo es una cara 3D. Llega como malla, no como sólido. |
| **SketchUp** | SketchUp (no la versión web gratuita) | Es un archivo **.dae** (Collada). |

### SketchUp

SketchUp no deja escribir su formato propio (.skp): es un formato cerrado. El .dae es el que
SketchUp importa con las unidades puestas: **Archivo → Importar** y elegir el archivo .dae.

Si se ven las aristas de todos los triángulos, seleccionar todo y aplicar **Suavizar aristas**
(Soften/Smooth Edges).

**Qué versión de SketchUp sirve** (relevado en octubre de 2026; Trimble cambia los planes seguido):

| Versión | Dónde corre | ¿Importa el .dae? | Costo |
|---|---|---|---|
| SketchUp Free | Web | **No**: solo abre .skp e imágenes (tampoco STL ni DXF) | Gratis |
| SketchUp Make 2017 | Escritorio (Windows/Mac) | Sí | Gratis, pero discontinuado: ya no se actualiza |
| SketchUp Go | Web y iPad | Sí | Pago |
| SketchUp Pro / Studio | Escritorio | Sí (y también DXF y STL) | Pago (hay licencias educativas) |
| SketchUp for Schools | Web | Sí | Gratis, solo para escuelas primarias y secundarias |

Sin licencia, lo más práctico es **SketchUp Make 2017**.

Los ejes de la aplicación tienen los mismos nombres y colores que en SketchUp: **x** roja,
**y** verde (profundidad) y **z** azul (hacia arriba). Lo que acá se estira «en z», en SketchUp
también está en z.

### Autodesk Fusion (uso personal)

La licencia gratuita de uso personal importa **STL** y **OBJ**; el **.dae no** y el **DXF**
solo en 2D (el nuestro es 3D, no sirve). Conviene el **STL**:

- **Insertar → Insertar malla** (Insert → Insert Mesh) y elegir **milímetros** en el diálogo:
  así queda en tamaño real (ni el STL ni el OBJ guardan las unidades).
- El STL viene con z hacia arriba (como en esta aplicación y en SketchUp); el OBJ, con y hacia
  arriba. Si la pieza aparece acostada, se endereza en el mismo diálogo de Insertar malla.
- Llega como malla. Para convertirla en sólido (Malla → Convertir malla) exportar en
  resolución **media o baja**: Fusion no convierte bien mallas de decenas de miles de triángulos.

### Resolución

- **Completa**: la malla tal como se ve en pantalla.
- **Media** y **Baja**: vuelven a armar el cuerpo con menos triángulos y le aplican las mismas
  fuerzas; la forma y la topología son las mismas y el archivo pesa mucho menos.

El menú muestra cuántos triángulos va a tener el archivo. SketchUp se pone lento por encima de
los 100.000: para esos casos conviene la resolución media o baja.
