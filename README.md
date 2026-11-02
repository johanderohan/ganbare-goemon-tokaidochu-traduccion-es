# Ganbare Goemon: Tōkaidōchū Ōedo Tengurigaeshi no Maki — Traducción al español

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/nintendo-ds/ganbare-goemon-tokaidochu)**.

Traducción al **español de España** de *Ganbare Goemon: Tōkaidōchū Ōedo
Tengurigaeshi no Maki* (がんばれゴエモン 東海道中 大江戸天狗り返しの巻, Nintendo DS,
Konami, 2005), la aventura de Goemon y Ebisumaru por el camino del Tokaido, que
solo salió en Japón. Es una traducción **directa del japonés**.

La traducción se reparte como **parche**: no incluye el juego. Necesitas tu propia
copia de la versión japonesa para aplicarlo.

## Estado

Última versión: **[v1.1](../../releases/tag/v1.1)**.

| Parte | Estado |
|---|---|
| Historia: apertura, juicios, escenas de los ocho actos, final y escenas de libro de cada zona | **Traducida entera** |
| Diálogos de pueblos, tiendas y casas de comidas, recados, concursos, dojos, cameos, ayudas de mecanismos y mensajes del sistema (guardar, datos, postas del camino) | **Traducidos enteros**: 3.373 grupos de diálogo |
| Gráficos con texto: título y submenús, selección de datos, Sí/No, opciones de sonido, pausa (con la pantalla de controles), placas de armas y objetos, nombres de hablante, placas de zona, sellos del minimapa, mapa del Tokaido con sus 57 postas, cartela y títulos de los capítulos, selección de personaje, minijuegos, jefes e Impact, precios de las cartas, placas de destino del porteador, minijuego del torno (tablón, indicadores, botones, arcillas y rangos), «¡N.º CAPÍTULO SUPERADO!», fin de partida y «JEFE» | **Redibujados en castellano** |
| Caracteres españoles | **á é í ó ú ü ñ Á É Í Ó Ú Ü Ñ ¡ ¿ « »** |

El original dibuja el texto en vertical en las escenas de libro y con una letra
japonesa de 16 px en el resto. El parche añade una letra latina de 8 px con el mismo
color y grosor de trazo que la japonesa y 300 pares de letras en una sola celda para que
el castellano quepa en los guiones. Las páginas se reparten de nuevo en cada caja sin
tocar voces, pausas, condiciones ni menús, y el libro de las escenas se lee de izquierda
a derecha.

Se mantienen como en el original, por ser imagen de marca o decorado: el logotipo del
título, el logotipo de Konami, el logotipo de Quarth (que ya está en inglés) y los
carteles dibujados dentro de algunas ilustraciones (el de busca y captura del libro de la
apertura y el letrero del juicio). El texto de esas escenas explica lo que dicen.

### Comprobaciones y trabajo pendiente

Se ha jugado en emulador (DeSmuME) **desde partida nueva** el principio del juego:
título y submenús, selección de datos, la apertura completa, el juicio, la prisión, el
pasadizo con su puzle de la cuerda y la llegada a Hagure (Edo), con sus vecinos, la casa
de té, la tienda de salsa de soja, la casa de comidas, la pausa con todas sus pestañas,
guardar, volver al título y cargar. Las escenas de libro del final de cada acto y el
final se han visto en el emulador por una ruta de prueba dirigida. Lo añadido en la v1.1
(porteador, minijuego del torno, rótulos de fin de capítulo y fin de partida) se ha
visto en el emulador; el fin del capítulo 1 y el fin de partida, jugando, y lo demás, con
pruebas dirigidas. Los nombres de hablante nuevos (Plasma, Kensuke, los Marble) solo se
han visto en pruebas dirigidas. **El resto del juego
(actos 2 a 8, sus pueblos, tiendas y jefes) no se ha jugado**: sus textos se han
traducido, revisado y comprobado con una auditoría automática que lee la ROM montada y
verifica los límites de cada caja y de cada guion, los caracteres, que se conservan
todos los controles del motor y la estructura de los ficheros. Un jugador está jugando
la v1.0 en consola real (sus avisos dieron lugar a la v1.1); nosotros no la hemos probado
en consola.

La traducción y la revisión se han hecho con ayuda de inteligencia artificial, con
biblia de personajes y términos, revisión editorial cruzada de todo el texto, una pasada
de coherencia entre zonas y pruebas en emulador, pero **sin revisión humana
independiente**. Si encuentras errores, abre una incidencia.

Pendiente o conocido:

- Los actos 2 a 8 no se han recorrido jugando: puede haber cortes de página mejorables o
  algún cuadro que no se haya visto nunca en pantalla.
- Algunas pestañas y sellos pequeños llevan la palabra partida con guion («CONTRO-LES»,
  «SALI-DA») porque no caben en una línea.
- «ryo» se ve pequeño en la ficha del diario y en los precios de la carta de las casas de
  comidas.
- No se ha completado ninguna compra con dinero en el emulador (sí se han visto la carta,
  sus fichas y la respuesta de la tabernera cuando no alcanza el dinero).
- La explicación de controles de los combates de Impact (vista en el menú de minijuegos)
  y la prueba de sonido siguen en japonés.
- El modo de descarga Impact (DS Download Play) conserva sus menús en japonés. La
  descarga inalámbrica no se ha probado.

## Cómo aplicar el parche

1. Descarga el parche `.xdelta` de la sección **[Releases](../../releases)**.
2. Consigue tu copia del juego en versión **japonesa**. El parche solo funciona con
   esa versión exacta.
3. **Comprueba que tu copia es la correcta** antes de nada:

   | | |
   |---|---|
   | Archivo | `Ganbare Goemon - TokaiDouchuu Ooedo Tengurigaeshi no Maki (Japan).nds` |
   | Tamaño | 67.108.864 bytes (64 MB) |
   | MD5 | `0408f68bbda4144673c54c550f76f4e2` |

   ```bash
   md5sum "Ganbare Goemon - TokaiDouchuu Ooedo Tengurigaeshi no Maki (Japan).nds"     # Linux
   md5 "Ganbare Goemon - TokaiDouchuu Ooedo Tengurigaeshi no Maki (Japan).nds"        # macOS
   CertUtil -hashfile "Ganbare Goemon - TokaiDouchuu Ooedo Tengurigaeshi no Maki (Japan).nds" MD5   # Windows
   ```

   Si no coincide, el parche fallará o dará un resultado corrupto.
4. Aplica el parche con una de estas herramientas:
   - **Windows**: [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases)
   - **Linux / macOS**: `xdelta3 -d -s "juego original.nds" parche.xdelta "juego traducido.nds"`
5. Para **v1.1**, comprueba que la ROM resultante tiene MD5
   **`1bc98d921496fda3998c046773a101d8`** (67.108.864 bytes). El parche se aplica
   siempre sobre la ROM japonesa original, no sobre una versión anterior traducida.
6. Carga la ROM resultante en tu emulador o flashcard preferidos.

## Cambios

- **v1.1**: traduce los gráficos que seguían en japonés: nombres de hablante que faltaban
  (Plasma, Kensuke, los Marble…), placas de destino del porteador, el minijuego del torno
  de Kanagawa entero (también las descripciones de arcilla), el rótulo de fin de capítulo,
  la pantalla de fin de partida y el rótulo «JEFE». Gracias al jugador que avisó.
- **v1.0**: primera versión pública.

## Créditos

- Traducción, fuente y herramientas: johanderohan.
- La letra latina de los diálogos deriva de DejaVu Sans Mono Bold (licencia de las
  fuentes Bitstream Vera y DejaVu, de uso libre).
- Los rótulos gráficos usan Fira Sans, © 2012-2018 The Mozilla Foundation, Telefónica
  S.A., Carrois Corporate GbR y bBox Type GmbH (licencia SIL Open Font License 1.1).

## Aviso

Este proyecto es una traducción hecha por afición, sin ánimo de lucro y sin relación
alguna con Konami. Aquí no se distribuye el juego ni ninguna parte de él: solo un parche
que modifica una copia que ya tengas.

Si eres el titular de los derechos y quieres que retire esto, abre una incidencia
y lo hago.
