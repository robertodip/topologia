# Topología

Arq. Roberto Dip

Una aplicación para ver, en 3D, qué cambia y qué no cuando un cuerpo se deforma como si
fuera de goma: estirar, torcer, doblar o inflar no cambian su topología; cortar o perforar,
sí. Al costado, un panel cuenta los vértices, aristas y caras, y muestra que esos números
no se mueven mientras el área y el volumen sí.

Es gratis para estudiar y enseñar (ver la licencia, más abajo).


## Cómo abrirla

**Opción 1 — En línea (lo más fácil).** Abrí este enlace en Edge o Chrome:

    https://robertodip.github.io/topologia/

No hay que instalar nada. Hace falta internet solo para abrirla.

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


## Primeros pasos

- **Arriba, dos pestañas:** *Superficies* (hojas planas y la cinta de Möbius) y
  *Volúmenes* (cubo, prismas, cilindro, esfera, toroide).
- **Mover la vista:** arrastrar con el mouse para girar, la rueda para acercar, el botón
  derecho para desplazar.
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

## El panel de la derecha

- **No cambian (topología):** vértices V, aristas A, caras C, la característica de Euler
  χ = V − A + C, el género (cantidad de agujeros), si es cerrada y si es orientable.
  Debajo dice a qué figura es **equivalente** el cuerpo: una esfera, un toro, un disco…
- **Cambian (geometría):** área y volumen, con el porcentaje respecto del original.

## Guardar el modelo

Menú **Archivo → Exportar como**: STL (impresión 3D), OBJ, DXF o SketchUp (.dae), en
milímetros. Los detalles de cada formato y cómo abrirlos en SketchUp, Fusion o Blender están
en **MANUAL.md** (se abre con el Bloc de notas).

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
