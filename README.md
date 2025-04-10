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

- Cerebro: Raspberry Zero W. Esto se podría sustituir por un
  microcontrolador, pero nos obligaría a hacer más cosas en la parte de
  programación.

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

| Ítem                                                                            | Precio (US\$) |
|:--------------------------------------------------------------------------------|--------------:|
| Tres Baterías 18650, mejor para 10 Ah                                           |            15 |
| Tres protectores de batería o PCM (sobredescarga, sobretensión y cortocircuito) |             3 |
| Sistema de gestión de bateria (BMS) de DIY More MCP73871                        |             3 |
| Step-up / step-down TPS63070                                                    |             1 |
| Raspberry Pi Zero W                                                             |            15 |
| Receptor (Unicore UM980)                                                        |          80\* |
| Coaxial corto MMCX (macho) - SMA (hembra)                                       |             2 |
| Antena de plato                                                                 |            55 |
| Interruptor (e.g., touch TTP223)                                                |             1 |
| Disipadores                                                                     |             5 |
| Caja (registro eléctrico, de comida)                                            |             5 |
| Gastable, accesorios varios, tornillería, cables, conectores                    |            10 |
| **Total**                                                                       |       **195** |

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
![](img/aplic_15_mesa_IMG_20250409_145023.jpg) ![](img/qr.jpg)

## Ver también

<https://geofis.github.io/mdt-campus-uasd-gnss-bajo-costo/presentaciones/III-Congreso-IDI-XXIII-JIC-nov24.html>
