Armemos receptores GNSS
================
José Ramón Martínez Batlle

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

-   Módulo principal: placa con módulo receptor GNSS (estoy inclinado a
    Unicore o Quectel, pero hay muchos otros a buen precio, como Bynav y
    ComNav).

-   Cerebro: Raspberry Zero W. Esto se podría sustituir por un
    microcontrolador, pero nos obligaría a hacer más cosas en la parte
    de programación.

-   Alimentación de energía:

    -   Circuito de carga de batería. Aunque estoy sugiriendo armar base
        fija para interiores, si le creamos un circuito de carga de
        batería, la base no será vulnerable a fluctuaciones de voltaje o
        cortes de luz, y podremos sacarla al campo con más facilidad
        (instalé una en el FC-203 que funciona 24/7, y la saco al campo
        regularmente).
    -   Regulador, tanto step-up (elevador de voltaje) como step-down
        (reductor de voltaje).
    -   Baterías, normalmente, uso la 18650, de ión de litio, 3.7V. Las
        venden en la 30 de Marzo. En este caso, con tres sería
        suficiente.

-   Caja protectora. Uso cajas de registro eléctrico, cuyas dimensiones
    suelen ser variables, pero normalmente
    ???????????????????????????????????????

-   Antena GNSS, preferiblemente de plato.

-   Cables, conectores JST: esto puede variar de un proyecto a otro,
    pero sí son imprescindibles el cable de la antena a la caja del
    receptor normalmente de 3 metros (LMR195 o RG174 con terminal TNC en
    una punta y SMA macho en la otra), un pequeño cable dentro de la
    caja, de 5 a 8 cm de longitud, con terminales SMA hembra en un lado
    y en la otra punta el terminal que use el receptor, normalmente MMCX
    o SMA (este pequeño cable dirige la señal desde la parte de afuera
    de la caja hacia la tarjeta del módulo GNSS), y cables de energía
    (20 AWG) cortos que van dentro de la caja. Los conectores JST son
    cómodos para armar y desarmar el equipo cuando haya que dar
    servicio.

-   Soportes y tornillería para estabilizar el proyecto dentro de la
    caja.

-   Terminal USB e interruptor (el interruptor también podría ser touch,
    capacitivo).

-   Montaje tipo V (macho y hembra).

-   Tornillos varios, M\*.

-   Herramientas útiles pero no imprescindibles, porque yo las puedo
    aportar: crimpadora de cables para armar conectores JST, crimpadora
    para cables coaxiales y conectores, soldador, estaño, flux, pinzas
    de corte, y otras herramientas.
