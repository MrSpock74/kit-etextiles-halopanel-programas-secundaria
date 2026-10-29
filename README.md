# Kit e-Textiles (HaloPanel): programas de ejemplo para Secundaria

Programas de las 14 lecciones del tutorial del kit de costura electrónica ACEBOTT TA648 (placa HaloPanel), listos para cargar en la placa y para abrir y modificar en el editor.

Material de apoyo de la formación del profesorado sobre el **Código Escuela 4.0** (CEP de Bollullos del Condado). La ficha didáctica del kit, con ejemplos por materia, está en el Google Sites del proyecto: https://sites.google.com/g.educaand.es/codigoescuela40-iesmurillo/kit-e-textiles

Tutorial completo del fabricante (PDF, 118 páginas): [tutorial/tutorial-kit-textil-avanzado.pdf](tutorial/tutorial-kit-textil-avanzado.pdf)

## Cómo usarlos

1. Conecta la placa por USB y pulsa **Reset dos veces** hasta que los NeoPixels se pongan en verde. Aparece una unidad llamada `CPLAYBOOT`.
2. Descarga el `.uf2` de la lección desde la carpeta [`uf2/`](uf2/) y arrástralo a esa unidad. La placa se reinicia con el programa.
3. Para **ver y modificar** el programa: cada `.uf2` lleva dentro su código fuente. Ábrelo en el editor https://acebott.com/halopanel/ (Chrome o Edge).

## Programas

| Archivo | Lección | Qué hace | Extensiones del proyecto |
|---|---|---|---|
| `halopanel-lesson_1.uf2` | 1 | Luces RGB: secuencia de colores en el anillo | heart-rate-sensor* |
| `halopanel-lesson_2.uf2` | 2 | Botones A y B cambian el color | heart-rate-sensor* |
| `halopanel-lesson_3.uf2` | 3 | Zumbador: melodía con funciones | heart-rate-sensor* |
| `halopanel-lesson_4.uf2` | 4 | Luces controladas por el sensor de luz | heart-rate-sensor* |
| `halopanel-lesson_5.uf2` | 5 | Alarma de temperatura | heart-rate-sensor* |
| `halopanel-lesson_6.uf2` | 6 | Detección de sonido | heart-rate-sensor* |
| `halopanel-lesson_7.uf2` | 7 | Acelerómetro: inclinación por ejes | heart-rate-sensor* |
| `halopanel-lesson_8.uf2` | 8 | Piano táctil con cinta de cobre | heart-rate-sensor* |
| `halopanel-lesson_9.uf2` | 9 | Servo en el pad A1 | servo |
| `halopanel-lesson_10.uf2` | 10 y 14 | LED externo en A1 (la lección 14 reutiliza este archivo) | servo |
| `halopanel-lesson_11.uf2` | 11 | Módulos RGB WS2812 en A1 | WS2812 |
| `halopanel-lesson_12.uf2` | 12 | Sensor de pulso | WS2812, heart-rate-sensor |
| `halopanel-lesson_13_Motherboard-1.uf2` | 13 | Infrarrojos: placa **emisora** | WS2812, heart-rate-sensor, cable |
| `halopanel-lesson_13_Motherboard-2.uf2` | 13 | Infrarrojos: placa **receptora** | (solo las incluidas) |

\* Estos proyectos declaran la extensión del sensor de pulso aunque no la usan.

## Antes de usarlos en clase

- **Extensiones desde GitHub.** `heart-rate-sensor`, `WS2812` y `cable` se descargan de GitHub al abrir el proyecto en el editor y aparecen como "no aprobada por Microsoft". Si la red del centro bloquea GitHub, el proyecto puede no abrirse. Cargar el `.uf2` directamente en la placa no necesita red. Se recomienda probar antes en la red del centro.
- **Servos:** alimentar con pilas, no con el USB.
- **Sensor de pulso:** es didáctico, no médico.

## Erratas del tutorial

- **Lección 8:** los pads A6 y A7 tocan los dos 440 Hz. La nota de A7 debería ser algo más aguda (unos 495 Hz).
- **Lección 13:** el anillo blanco del receptor se borra a los 100 ms y apenas se ve.
- **Lección 7:** la tabla dice que Z apunta hacia arriba, pero marca −1024 con la placa boca arriba.

Se pueden usar como ejercicio: "encuentra el error y corrígelo".

## Autoría y licencias

- El tutorial y los programas `.uf2` proceden del material de **ACEBOTT** (kit TA648, tutorial V1.2) y son suyos. Se incluyen sin modificar, con fines educativos.
- Este README y el resto de documentación: Manuel Romero Fraidía (IES Murillo, Sevilla), licencia [CC BY-NC-SA 4.0](LICENSE.md).
