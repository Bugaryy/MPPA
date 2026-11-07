# MPPA Panamá Pacífico 3D

Modelo 3D interactivo del **Aeropuerto Internacional Panamá Pacífico (MPPA)**, la antigua base aérea de Howard, en Arraiján, Panamá. Sirve para estudiar el aeródromo: pista, calles de rodaje, plataformas, edificios, luces, terreno y espacio aéreo, con los datos de la AIP de Panamá.

**Autor:** Delta Charlie · [github.com/Bugaryy](https://github.com/Bugaryy)

> ⚠️ **Herramienta de estudio. No apta para uso operacional.** Para cualquier operación, consulta siempre la AIP de Panamá vigente y los NOTAM.

---

## Cómo abrirlo

Todo va dentro de un solo archivo, `index.html`: código, datos, terreno y texturas satelitales. No hace falta instalar nada.

1. Abre `index.html` en un navegador moderno (Chrome, Edge, Safari o Firefox), en computadora o celular.
2. La página necesita internet solo para cargar la biblioteca three.js y las tipografías desde sus CDN.

## Controles

| Acción | Computadora | Celular |
|---|---|---|
| Girar la vista | Arrastrar con el botón izquierdo | Arrastrar con un dedo |
| Mover el mapa | Arrastrar con el botón derecho | Arrastrar con dos dedos |
| Acercar / alejar | Rueda del mouse | Pellizcar |
| Ver información | Clic sobre el elemento | Tocar el elemento |

**Vista desde la torre:** la cámara queda fija dentro de la cabina de la TWR. Arrastra para girar 360° y usa la rueda o el pellizco para acercar. Para salir, usa el botón **Salir de TWR**, la tecla Esc o cualquier otra vista.

## Funciones

- **Información al tocar:** pista, calles de rodaje, plataformas, hangares, terminal, torre, PAPI, mangas de viento, sensores MET, tanques de combustible y cerros, cada uno con sus datos de la AIP.
- **Buscador:** encuentra y resalta cualquier elemento por nombre o letra (A, B, D, E, F, G…).
- **Panel AIP:** datos del aeródromo, frecuencias, espacio aéreo, circuitos de tránsito, ruido, aves y procedimientos.
- **Capas:** se pueden activar y desactivar.
  - Imagen satelital y etiquetas.
  - Edificios.
  - Pista y calles vectoriales, letreros y puntos de espera.
  - Luces aeronáuticas.
  - Franja, RESA y CWY.
  - Cerros.
  - ATZ (2100 ft) y CTR (3000 ft).
  - Circuitos de tránsito (al este del AD).
  - Modo nocturno.
- **Vistas rápidas:** General, Final RWY 18, Final RWY 36, Desde la TWR, Plataformas y hangares, Cerros Cabra y Galera, Cerro Ancón y Circuitos.

## Contenido del modelo

**Pista 18/36:** mide 2591 × 45 m (ASPH, PCN 70/F/C/X/U) y tiene una pendiente real entre THR 36 (6.09 m) y THR 18 (15.24 m). Las señales de umbral, designadores, TDZ, punto de visada, eje y fajas laterales siguen el estándar OACI. Tiene luces de borde cada 60 m, luces de umbral y de extremo, y PAPI de 3.1° (RWY 18) y 3.0° (RWY 36).

**Calles de rodaje A, B, D, E, F y G:** de 23 m, trazadas sobre la imagen satelital, con señales de eje y borde, puntos de espera, eje mejorado y luces azules. También están las calles del lado oeste sin designador, entre ellas la paralela cerrada que el ADC marca con X.

**Plataformas:** Norte, Central y Sur.

**Edificios:** terminal, hangar del SENAN, hangares con techo de bóveda, oficinas, SEI, tanques de combustible y la torre de control (218 ft / 66.45 m AMSL).

**Terreno y cerros:** el relieve incluye los cerros Cabra, Galera, Guayabo, Ancón, Sosa, Farfán y Miñón, además de la costa y el mar.

**Espacio aéreo:** ATZ y CTR construidos con los límites publicados en AD 2.17.

## Fuentes y método

- **Datos aeronáuticos:** AIP Panamá AD 2.6-MPPA (AD 2.1 a 2.24, ADC y carta CTR).
- **Imagen satelital:** 10 capturas de Google Maps, unidas automáticamente y georreferenciadas con las coordenadas de los umbrales del AIP. En el área del aeródromo la escala es de unos 1.07 m/px.
- **Calles, plataformas y edificios:** trazados sobre esa imagen y revisados superponiéndolos a ella.

## Limitaciones y diferencias con el AIP

- **Rumbo de la pista.** El AIP publica el mismo meridiano para ambos umbrales y un rumbo de 1.97° / 181.97°. Las imágenes muestran que la pista no es exactamente norte-sur. El modelo usa 177.4° verdadero para la RWY 18 (181.97° magnético − 4.6° de VAR W), que coincide con lo medido en la imagen.
- **Faro (ABN).** El AIP publica su coordenada 1.5 km al este, sobre el agua. El ADC lo ubica junto a la torre, y así se representa.
- **Frecuencia de torre.** El ADC rotula TWR 119.7. Se usa la de AD 2.18: 118.900 MHz.
- **Relieve.** Es aproximado: se construyó con las elevaciones de AD 2.10 y las cotas de la carta CTR. No es un modelo digital de elevación.
- **Edificios.** Las alturas son estimadas porque no se publican.
- **Puntos de espera.** Su distancia es aproximada, salvo en la TWY D, donde se midió en la imagen.
- **Imagen satelital.** Fuera del aeródromo es de menor resolución.

## Créditos

- Autor: **Delta Charlie** · [github.com/Bugaryy](https://github.com/Bugaryy)
- [three.js](https://threejs.org) — licencia MIT.
- Tipografías IBM Plex Sans Condensed y IBM Plex Mono — SIL Open Font License 1.1.
- Información aeronáutica: AIP de Panamá, Autoridad Aeronáutica Civil.
- Imágenes satelitales: Google Maps y sus proveedores.

## Licencia

Software propietario, con todos los derechos reservados. Puedes usarlo solo para estudio personal. Copiarlo, redistribuirlo, modificarlo o usarlo comercialmente requiere autorización por escrito del autor. Consulta el archivo [LICENSE](LICENSE).

Copyright © 2026 Derek Cuan ("Delta Charlie").
