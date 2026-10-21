# Ruta Andina

Juego de carreras 3D en el navegador, ambientado en Chile: la cordillera de los Andes, la Alameda de Santiago, las curvas de Los Caracoles y la Carretera Austral. Además trae un **Desafío 4x4** de cuatro etapas solo para camionetas.

Funciona con un solo archivo (`index.html`). Usa Three.js desde un CDN, así que necesita conexión a internet.

## Cómo jugar

- **En línea:** https://mati47589.github.io/ruta-andina/
- **En tu computador:** abre `index.html` con Chrome, Edge o Firefox.
- **Ir directo a un mapa:** agrega `#mapa=alameda`, `#mapa=caracoles`, `#mapa=austral` o `#mapa=cordillera` al final de la dirección (o `#mapa=x4_rocas`, `x4_rio`, `x4_dunas`, `x4_barro` para las etapas 4x4).

## Mapas

| Mapa | Lugar | Qué tiene |
|---|---|---|
| Circuito Cordillera | Valle del Aconcagua | Carretera de montaña con araucarias, palmas chilenas y la Laguna del Inca. 3 vueltas. |
| La Alameda | Santiago Centro | Carrera callejera por la calzada sur de la Alameda, de un solo sentido, con su pista "solo bus", y vuelta por la Costanera. Al otro lado del bandejón central (dos hileras de plátanos orientales, paseo de baldosas, bancas, quioscos, accesos a la Línea 1 del Metro y O'Higgins a caballo frente a La Moneda) corre la calzada norte con micros, taxis y colectivos hacia el poniente. Calles que la cruzan con cebras y semáforos, y en su orden real: Torre Entel, La Moneda, Universidad de Chile, San Francisco, Biblioteca Nacional, cerro Santa Lucía, Universidad Católica, GAM y Plaza Baquedano. La vuelta va por Cardenal Caro, junto al Mapocho: paseo de ladrillo con balaustrada, muros de piedra del río, puentes de arco, el Parque Forestal con el Museo de Bellas Artes y la Fuente Alemana, la Estación Mapocho, y al otro lado Av. Santa María con su tránsito y las casas de colores de Bellavista. 3 vueltas. |
| Los Caracoles | Paso Los Libertadores | Horquillas numeradas subiendo hacia Portillo, galerías antinieve, hielo, derrumbes y camiones a Argentina. 2 vueltas. |
| Carretera Austral | Lago General Carrera | Camino de ripio entre coigües, puentes de madera sobre esteros, barro, pozas, troncos caídos, vacas sueltas y las Capillas de Mármol. 3 vueltas. |

## Una ciudad viva

- **Gente:** santiaguinos que caminan por las veredas, el paseo del bandejón, la orilla del Mapocho y los senderos del Parque Forestal, cada uno con su ropa, su paso y su ritmo.
- **Comercio:** locales a nivel de calle con letrero, vitrina y toldo (farmacia, botillería, fuente de soda, salón de té, empanadas, casa de cambio, peluquería, óptica, librería, quiosco de diarios y más, y alguna cortina metálica cerrada). Al atardecer se encienden.
- **Semáforos que cambian:** los del otro lado de la Alameda pasan de verde a amarillo y rojo, y las micros y autos se detienen en fila y arrancan con el verde. Los de la carrera parpadean en amarillo (calle cortada).
- **Árboles con hojas:** las copas están hechas de hojas sueltas que dejan pasar la luz y se mecen con el viento, en todos los mapas.
- **Aire de Santiago:** una capa de esmog café-grisácea sobre el horizonte, más espesa con cielo despejado.
- **Sonido ambiente:** rumor del tránsito y bocinas lejanas en la ciudad, el Mapocho corriendo, pájaros en los parques y bosques, el chucao en el sur y el viento en la montaña.

## Desafío 4x4 (solo camionetas)

Etapas contra el reloj con obstáculos de verdad. Antes de cada etapa hay que **preparar la camioneta**, y esa preparación cambia la dificultad: el taller dice si la etapa queda Fácil, Media, Difícil o Muy difícil y qué te falta.

| Etapa | Lugar | El desafío | Qué conviene |
|---|---|---|---|
| 1 · Quebrada de Macul | Precordillera de Santiago | Bolones, escalera de roca, laderas inclinadas y "El Escalón" de 50 cm | Bloqueos, neumáticos grandes, presión baja, recorrido largo, protecciones |
| 2 · Cajón del Maipo | Río Colorado | Un vado de 45 cm y otro de 1 m con corriente, barro en las orillas | **Snorkel** (sin él, el motor se ahoga), neumáticos AT/MT, huinche |
| 3 · Dunas de Atacama | Desierto de Atacama | Arena blanda entre dunas | **Presión baja** (con 35 psi el neumático se entierra), ir con impulso |
| 4 · Barro de Nahuelbuta | Cordillera de Nahuelbuta, con lluvia | Pozones de barro profundo, troncos y una cuesta resbaladiza | **Neumáticos de barro (MT)**, bloqueos, huinche |

**Preparación:** tipo de neumático (carretera, todo terreno, barro, competencia), medida (31" a 37"), presión (35 a 12 psi), bloqueos de diferencial, control de tracción, relación de corona, suspensión (original, levantada, recorrido largo), barra estabilizadora, snorkel, huinche y protecciones. Se guarda por etapa y por camioneta.

**Física 4x4:** cada rueda con su suspensión y contacto con el terreno, diferenciales abiertos o bloqueados, caja de transferencia 2H/4H/4L (reductora 2,72:1), convertidor de torque, hundimiento y surco en arena y barro según la presión, neumático que trepa por el canto de los escalones, flotación y corriente en el río, toma de aire que se inunda y huinche que tira más lento mientras más carga.

**Controles 4x4:** `F` 2H/4H/4L (la reductora entra detenido) · `L` bloqueos · `G` huinche al anclaje con eslinga amarilla más cercano · `T` control de tracción · `R` rescate al último control (+30 s; si te repites en el mismo tramo, un tractor te remolca pasado el obstáculo: +60 s).

Hay medallas de oro, plata y bronce por etapa, y al final te da un consejo sobre lo que le faltó a tu preparación.

## Sonido y música

Todo se genera en el momento con Web Audio, sin archivos de audio: el juego sigue siendo un solo `index.html`.

- **Motores de verdad:** cada motor se sintetiza explosión por explosión, con su número de cilindros y su orden de encendido (el V8 cruzado del Cóndor GT suena desparejo, como uno real), escape con resonancia y silenciador, turbo con silbido y descarga ("pssh") al soltar, traqueteo del diésel y petardeos. El escape deportivo y la preparación por etapas se escuchan.
- **Arranque, cambios y limitador:** marcha y tos antes de la largada, golpe de la caja en cada cambio, petardeo al subir a fondo en el rally y el GT, golpe de acelerador al reducir y corte al llegar al limitador.
- **Los demás también suenan:** rivales y tránsito (autos, micros y camiones) con efecto Doppler, paneo estéreo y distancia. En el 4x4 se oye el motor del huinche.
- **Música por mapa:** huayno con quena y charango en la Cordillera, cumbia chilena en La Alameda, tema tenso con arpegios en Los Caracoles y cueca con guitarra en la Carretera Austral; las etapas 4x4 usan el tema andino (roca y río), el tenso (dunas) y la cueca (barro). Hay otro tema tranquilo para el menú. Suma instrumentos a medida que vas más rápido, queda bajo el motor y se apaga suave al pausar.
- **Controles:** `N` activa o desactiva solo la música (también hay botón en el menú y en la pausa); `M` silencia todo.

## Peligros del camino

Cambian en cada carrera según la dificultad y el clima: baches (pueden doblar una rueda y desalinear la dirección), pozas (aquaplaning), manchas de aceite, hielo, nieve, barro, ripio suelto, tapas de alcantarilla, lomos de toro, faenas con conos y una pista cerrada, derrumbes y troncos caídos. Además hay tránsito en ambos sentidos que frena, se corre a la orilla y toca la bocina.

## Taller

Cada auto se puede modificar y los cambios quedan guardados:

- **Pintura:** color, acabado (brillante, metalizado, mate, cromado), franjas y vidrios polarizados.
- **Ruedas:** llantas y su color, neumáticos (calle, deportivos, semi-slick, todoterreno, invierno) y altura.
- **Motor:** preparación por etapas, escape y relación de la caja.
- **Chasis:** suspensión (confort, deportiva, rally), frenos, peso y alerón.

El taller muestra cómo cambian la potencia, el 0–100, la velocidad máxima, el agarre y el frenado. Los neumáticos importan: los semi-slick vuelan en asfalto seco pero patinan con lluvia, y los de invierno son los únicos que agarran en el hielo.

## Autos

| Auto | Tracción | Potencia de fábrica |
|---|---|---|
| Taxi santiaguino | Delantera | 143 CV |
| Rally Estrella | 4x4 turbo | 299 CV |
| Camioneta 4x4 (doble cabina) | 4x4 diésel turbo | 204 CV |
| Camioneta corta (cabina simple) | 4x4 V6 bencina | 245 CV |
| Cóndor GT | Trasera | 408 CV |

## Controles

| Tecla | Acción |
|---|---|
| W / ↑ | Acelerar |
| S / ↓ | Frenar (mantén detenido para ir en reversa) |
| A / D | Dirección |
| Espacio | Freno de mano |
| E / Q | Subir / bajar cambio (caja manual) |
| C | Cambiar cámara: persecución, lejana, capó y **cabina** (al volante, con el tablero y el volante que gira) |
| Arrastrar el mouse / dedo | Mirar alrededor del auto, o dentro de la cabina (rueda o pellizco: acercar) |
| V | Centrar la cámara |
| R | Volver a la ruta (si estás volcado o con el motor destruido, llama a la grúa: +10 s) |
| 1 / 2 | ABS / control de tracción |
| M | Sonido (todo) |
| N | Música |
| Esc | Pausa |

También funciona con joystick y con controles táctiles en el celular.

## Cabina

Con la cuarta cámara manejas desde el asiento del conductor (a la izquierda, como en Chile): tablero con tacómetro, velocímetro y marcha que funcionan, volante que gira con la dirección, palanca, radio, paneles de puerta, asientos, parasoles y espejo. La cabeza se mece al frenar y en las curvas, y el horizonte se inclina con la carrocería. Funciona también en las camionetas del Desafío 4x4.

## Opciones

- **Modo:** carrera contra 5 rivales, o contrarreloj.
- **Dificultad:** Fácil, Normal, Difícil o Extrema (rivales más rápidos, más peligros y más tránsito).
- **Clima:** despejado, lluvia o nieve.
- **Hora:** mediodía, tarde dorada o arrebol (en Santiago se encienden las ventanas y los faroles).
- **Daños:** realistas (abolladuras, vidrios, motor, vuelcos), solo visuales o sin daños.
- **Calidad gráfica:** Alta, Media o Baja. La resolución se ajusta sola para mantener la fluidez. El terreno se dibuja por bloques (solo lo que ve la cámara) y los autos lejanos usan una versión simplificada, para que corra bien en computadores con gráfica integrada.
