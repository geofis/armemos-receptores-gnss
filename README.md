Armemos receptores GNSS
================
José Ramón Martínez Batlle

## Código QR de este repo

<img src="img/qr.jpg" style="width:50.0%" />

## Lista completa de materiales

Creé este repo para alojar la lista de materiales (BOM) requeridos para
armar receptores GNSS. El repo es igualmente un apoyo para talleres de
formación basados en aprendizaje práctico (manos a la obra, *hands-on*),
donde los y las participantes se dividirían en grupos idealmente de 3
personas para armar una base permanente de interiores, que a la vez sea
actualizable y expandible, y pensada para posibles adaptaciones de
movilidad futuras.

Esta alternativa es viable porque es relativamente fácil comenzar con un
proyecto que no requiera estrictamente la impermeabilización, pero
considerándola en primera instancia en el contexto del diseño expandible
para lograr una eventual necesidad portabilidad. El diseño para
interiores facilita muchas cosas en un taller de formación, pues lograr
la estanqueidad de una caja o implementar un circuito de alimentación
ininterrumpida, por ejemplo, suele ser desafiante.

La lista de partes sería básica (la imagen adjunta es un buen
complemento visual):

- Módulo principal: placa con módulo receptor GNSS (estoy inclinado a
  Unicore o Quectel, pero hay muchos otros a buen precio, como Bynav y
  ComNav).

- Módulo de control o computación, “cerebro”: Raspberry Zero W. Esto se
  podría sustituir por un microcontrolador, pero nos obligaría a hacer
  más cosas en la parte de programación. En el caso de una base para
  interiores, también se podría utilizar una PC, pero sería una solución
  energéticamente ineficiente.

- Alimentación de energía:

  - Circuito de carga de batería. Aunque estoy sugiriendo armar base
    fija para interiores, si le creamos un circuito de carga de batería,
    la base no será vulnerable a fluctuaciones de voltaje o cortes de
    luz, y podremos sacarla al campo con más facilidad (instalé una en
    el FC-203 que funciona 24/7, y la saco al campo regularmente).
  - Regulador, tanto step-up (elevador de voltaje) como step-down
    (reductor de voltaje).
  - Baterías, normalmente, uso la 18650, de ión de litio, 3.7V. Las
    venden en la 30 de Marzo. En este caso, con tres sería suficiente.

- Caja protectora. Uso cajas de registro eléctrico, cuyas dimensiones
  suelen ser variables, pero normalmente uso las de 130x80x70 mm. Pero
  cualquier envase de plástico para comida, que resista algo de
  temperatura y sea impermeable, servirá.

- Antena GNSS, preferiblemente de plato.

- Cables, conectores JST: esto puede variar de un proyecto a otro, pero
  sí son imprescindibles el cable de la antena a la caja del receptor
  normalmente de 3 metros (LMR195 o RG174 con terminal TNC en una punta
  y SMA macho en la otra), un pequeño cable dentro de la caja, de 5 a 8
  cm de longitud, con terminales SMA hembra en un lado y en la otra
  punta el terminal que use el receptor, normalmente MMCX o SMA (este
  pequeño cable dirige la señal desde la parte de afuera de la caja
  hacia la tarjeta del módulo GNSS), y cables de energía (20 AWG) cortos
  que van dentro de la caja. Los conectores JST son cómodos para armar y
  desarmar el equipo cuando haya que dar servicio.

- Soportes y tornillería para estabilizar el proyecto dentro de la caja.

- Terminal USB e interruptor (el interruptor también podría ser touch,
  capacitivo).

- Montaje tipo V (macho y hembra).

- Tornillos varios, M\*.

- Herramientas útiles pero no imprescindibles, porque yo las puedo
  aportar: crimpadora de cables para armar conectores JST, crimpadora
  para cables coaxiales y conectores, soldador, estaño, flux, pinzas de
  corte, y otras herramientas.

## Componentes del receptor GNSS mostrado en la demo

| Ítem | Precio (US\$) |
|:---|---:|
| Tres Baterías 18650, mejor para 10 Ah | 15 |
| Tres protectores de batería o PCM (sobredescarga, sobretensión y cortocircuito) | 3 |
| Sistema de gestión de bateria (BMS) de DIY More MCP73871 | 3 |
| Step-up / step-down TPS63070 | 1 |
| Raspberry Pi Zero W | 15 |
| Receptor (Unicore UM980) | 80\* |
| Coaxial corto MMCX (macho) - SMA (hembra) | 2 |
| Antena de plato | 55 |
| Interruptor (e.g., touch TTP223) | 1 |
| Disipadores | 5 |
| Caja (registro eléctrico, de comida) | 5 |
| Gastable, accesorios varios, tornillería, cables, conectores | 10 |
| **Total** | **195** |

<sup>\*</sup><small>Pagué ese precio, pero ahora está más caro. Hacen
ofertas regularmente.</small>

![](img/0_0_0_partes-general.jpg) ![](img/0_0_esquematico.png)
![](img/00_18650.jpg) ![](img/01_pcm-proteccion-bateria.jpg)
![](img/02_bms-diy-more-mcp7871.jpg) ![](img/03_TPS63070.jpg)
![](img/04_rpi-zero-w.jpg) ![](img/05_um980.jpg)
![](img/06_mmcx-sma.jpg) ![](img/07_antena-de-plato.jpg)
![](img/08_ttp-223.jpg) ![](img/09_disipadores.jpg) ![](img/10_caja.jpg)
![](img/aplic_00_gnss-deslizamientos.png)
![](img/aplic_01_hormigueros_0_IMG_20250325_164028.jpg)
![](img/aplic_01_hormigueros_mapa.png)
![](img/aplic_02_jardin-botanico-santiago.png)
![](img/aplic_03_puntos_uasd.jpg) ![](img/aplic_04_mdt_uasd.jpg)
![](img/aplic_05_repceptoresIMG_20241109_224524.jpg)
![](img/aplic_06_antenas_carro_IMG_20241110_114536.jpg)
![](img/aplic_07_antena_base_fc_IMG_20241116_140933.jpg)
![](img/aplic_08_receptor_base_arriba_IMG_20250126_211012.jpg)
![](img/aplic_09_receptor_base_abajo_IMG_20250126_211229.jpg)
![](img/aplic_10_mana_IMG_20231208_100215.jpg)
![](img/aplic_11_mana_IMG_20231208_121223.jpg)
![](img/aplic_12_hato_mayor_IMG_20241012_133700.jpg)
![](img/aplic_12_hato_mayor_Screenshot_2024-10-12-11-47-08-436.jpg)
![](img/aplic_13_playa_IMG_20241201_121708.jpg)
![](img/aplic_14_playa_IMG_20241201_121711.jpg)
![](img/aplic_15_mesa_IMG_20250409_145023.jpg)

## Ver también

<https://geofis.github.io/mdt-campus-uasd-gnss-bajo-costo/presentaciones/III-Congreso-IDI-XXIII-JIC-nov24.html>

## Diseños posibles y lista de componentes

> Ver ejemplos de componentes arriba.

> En todos los casos de asume que existe conectividad a Internet; si se
> requiriese transmisión/recepción por radio, a cada diseño habría que
> añadir un transmisor (base) o receptor (rover).

> En todos los casos, sobre todo en los equipos para el exterior, se
> necesitarán conectores, conductores (normales, tipo mm o AWG, y
> coaxiales), terminales (e.g. JST, SMA, u.Fl, MMCX, etc.), los cuales
> deberán considerarse en la lista de materiales.

### Base fija de interiores

- Receptor GNSS con puerto USB.

  - Alternativamente, si el receptor solo tiene terminal UART, se
    requiere adaptador UART-USB, e.g. FTDI, pero esto no es requerido si
    se usa microcontrolador en el lado computación.
  - Ver marcas de receptores arriba, pero los precios más competitivos
    los ofrecen Quectel, Unicore Communications y u-blox. En AliExpress,
    ocasionalmente hay ofertas de receptores SINOGNSS. Es importante que
    hagas tu propia búsqueda para que elijas lo que mejor se adapte a
    tus necesidades. Los criterios comúnmente son: consumo, número de
    frecuencias, eficiencia de disipación, tamaño.

- Unidad control o computador. Cualquiera de las siguientes opciones es
  válida, cada una con sus pros y sus contras:

  - PC Windows o Linux (GUI).
  - Raspberry Pi u otra marca de SBC (Linux, consola). En interiores no
    hay restricciones energéticas, así que puedes usar una Raspberry Pi
    4 o 3B+. Si necesitaras que el consumo fuese bajo, entonces
    Raspberry Pi Zero W.
  - Microcontrolador (e.g. ESP32).

- Cable USB. En interiores, cualquier cable USB común es válido (casi
  todos los receptores modernos usan USB-A en el extremo de la PC y
  Tipo-C en el extremo del receptor).

- (opcional) Si se requiere almacenamiento para posproceso, necesitarás
  un disco con suficiente espacio (mejor uno dedicado).

- Software: RTKBase, o directamente RTKLIB, o bibliotecas C++
  (e.g. bibliotecas GNSS de Sparkfun) si se usa microcontrolador

- Cuenta en rtk2go.com u Onocoy o Geodnet o crear un caster directamente
  (esto último obliga a exponer la IP pública, por lo que se recomienda
  usar un cliente VPN).

- Antena GNSS capaz de recibir las frecuencias que el receptor pueda
  procesar. La antena de plato es la mejor opción.

### Base móvil/exteriores

Misma lista que la anterior, con las siguientes particularidades:

- La unidad de control o cómputo sólo podría ser SBC o microcontrolador.

- Protección que sea resistente al polvo y al agua (estanqueidad
  garantizada, grado IP o *ingress protection*). Una caja de registro
  eléctrico, o similar, podría hacer el trabajo. Las cajas metálicas,
  aunque son más pesadas, disipan mejor el calor, lo cual es importante
  para el receptor y la unidad de control. Colocar un disipador de calor
  pasivo, tanto sobre el módulo del receptor, como sobre la CPU de la
  SBC o microcontrolador, es altamente recomendado.

- Añadir sistema de alimentación, que incluye:

  - Bateria(s) 3.7v (e.g. 18650)
  - Protection Circuit Module (PCM),
  - Battery Management System (BMS)
  - Step-up/step-down

### Rover (lógicamente, para exteriores) con alimentación propia

Casi los mismos componentes que la base móvil, pero con las
particularidades siguientes:

- En el caso de que el receptor tenga buen filtro, una antena de tipo
  *helix* puede funcionar.

- Software.

  - En el caso de usar SBC las opciones son limitadas, pero estoy usando
    [BashRTKStation](https://github.com/geofis/BashRTKStation/).
  - En el caso de usar microcontroldor, las bibliotecas GNSS de Sparkfun
    son las más recomendadas.

### Rover “híbrido”, con alimentación externa.

Se podría considerar un rover híbrido, similar al anterior, en el que
todo el módulo de alimentación externa podría sustituirse por un
powerbank.

## Proveedores sugeridos

- AliExpress
- Sparkfun
- DigiKey
- Mouser
- Adafruit
- ArduSimple
- Amazon
- eBay.
