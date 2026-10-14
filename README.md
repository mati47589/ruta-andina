# Ruta Andina

Juego de carreras 3D en el navegador, ambientado en Chile: la cordillera de los Andes, la Alameda de Santiago, las curvas de Los Caracoles y la Carretera Austral.

Funciona con un solo archivo (`index.html`). Usa Three.js desde un CDN, así que necesita conexión a internet.

## Cómo jugar

- **En línea:** https://mati47589.github.io/ruta-andina/
- **En tu computador:** abre `index.html` con Chrome, Edge o Firefox.
- **Ir directo a un mapa:** agrega `#mapa=alameda`, `#mapa=caracoles`, `#mapa=austral` o `#mapa=cordillera` al final de la dirección.

## Mapas

| Mapa | Lugar | Qué tiene |
|---|---|---|
| Circuito Cordillera | Valle del Aconcagua | Carretera de montaña con araucarias, palmas chilenas y la Laguna del Inca. 3 vueltas. |
| La Alameda | Santiago Centro | Carrera callejera entre muros de concreto: La Moneda, la Torre Entel, la Iglesia de San Francisco, el cerro Santa Lucía, el San Cristóbal, la Costanera Center, micros y colectivos. 3 vueltas. |
| Los Caracoles | Paso Los Libertadores | Horquillas numeradas subiendo hacia Portillo, galerías antinieve, hielo, derrumbes y camiones a Argentina. 2 vueltas. |
| Carretera Austral | Lago General Carrera | Camino de ripio entre coigües, puentes de madera sobre esteros, barro, pozas, troncos caídos, vacas sueltas y las Capillas de Mármol. 3 vueltas. |

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
| Camioneta 4x4 | 4x4 diésel | 204 CV |
| Cóndor GT | Trasera | 408 CV |

## Sonido y música

Todo se genera en el momento con Web Audio, sin archivos de audio: el juego sigue siendo un solo `index.html`.

- **Motores con carácter propio:** el taxi suena a cuatro cilindros sedán; el Rally Estrella tiene silbido de turbo, descarga ("pssh") al soltar el acelerador y petardeos; la camioneta es un diésel con traqueteo grave; el Cóndor GT es un V8 con su bamboleo y petardeos al subir de marcha. El escape deportivo y la preparación por etapas se escuchan.
- **Arranque, cambios y limitador:** marcha y tos antes de la largada, golpe de la caja en cada cambio, golpe de acelerador al reducir y corte de combustión al llegar al limitador.
- **Los demás también suenan:** rivales y tránsito (autos, micros y camiones) con efecto Doppler y paneo estéreo según por dónde pasan. Con el motor dañado falla, y destruido se apaga.
- **Música por mapa:** huayno con quena y charango en la Cordillera, cumbia chilena en La Alameda, tema tenso con arpegios en Los Caracoles y cueca con guitarra en la Carretera Austral. Hay otro tema tranquilo para el menú. Suma instrumentos a medida que vas más rápido y se apaga suave al pausar.
- **Controles:** `N` activa o desactiva solo la música (también hay botón en el menú y en la pausa); `M` silencia todo.

## Controles

| Tecla | Acción |
|---|---|
| W / ↑ | Acelerar |
| S / ↓ | Frenar (mantén detenido para ir en reversa) |
| A / D | Dirección |
| Espacio | Freno de mano |
| E / Q | Subir / bajar cambio (caja manual) |
| C | Cambiar cámara |
| R | Volver a la ruta (si estás volcado o con el motor destruido, llama a la grúa: +10 s) |
| 1 / 2 | ABS / control de tracción |
| M | Sonido (todo) |
| N | Música |
| Esc | Pausa |

También funciona con joystick y con controles táctiles en el celular.

## Opciones

- **Modo:** carrera contra 5 rivales, o contrarreloj.
- **Dificultad:** Fácil, Normal, Difícil o Extrema (rivales más rápidos, más peligros y más tránsito).
- **Clima:** despejado, lluvia o nieve.
- **Hora:** mediodía, tarde dorada o arrebol (en Santiago se encienden las ventanas y los faroles).
- **Daños:** realistas (abolladuras, vidrios, motor, vuelcos), solo visuales o sin daños.
- **Calidad gráfica:** Alta, Media o Baja. La resolución se ajusta sola para mantener la fluidez.
