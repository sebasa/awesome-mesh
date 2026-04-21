# Awesome Offgrid & Mesh [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> Una lista curada de recursos para **redes comunitarias, mesh y comunicaciones offgrid** — firmware, protocolos, software y servicios pensados para funcionar sin (o con poco) Internet.

Construida combinando los recursos de [MonteLibre — Recursos para redes comunitarias](https://montelibre.net/blog/recursos-para-redes-comunitarias/) y [moarpepes/awesome-mesh](https://github.com/moarpepes/awesome-mesh), reorganizada por categoría y con la licencia indicada cuando se conoce.

---

## Contenidos

- [Documentación](#documentación)
- [Protocolos de mesh](#protocolos-de-mesh)
  - [Routing](#routing)
  - [Stack](#stack)
- [Firmware y sistemas para routers](#firmware-y-sistemas-para-routers)
- [Sistemas operativos para self-hosting](#sistemas-operativos-para-self-hosting)
- [Hardware mesh y offgrid](#hardware-mesh-y-offgrid)
- [Software all-in-one para mesh](#software-all-in-one-para-mesh)
- [Comunicación — mensajería y VoIP](#comunicación--mensajería-y-voip)
- [Comunicación — redes sociales y P2P](#comunicación--redes-sociales-y-p2p)
- [Videollamadas y streaming](#videollamadas-y-streaming)
- [Multimedia](#multimedia)
- [Productividad y colaboración](#productividad-y-colaboración)
- [Educación offline](#educación-offline)
- [Mapas](#mapas)
- [Seguridad y privacidad](#seguridad-y-privacidad)
- [Comunidades](#comunidades)
- [Recursos adicionales](#recursos-adicionales)
- [No-código-abierto / source-available](#no-código-abierto--source-available)
- [Licencia](#licencia)

---

## Documentación

- [Wireless Mesh Networking](https://en.wikibooks.org/wiki/Wireless_Mesh_Networks) — Wikibook dedicado al tema.
- [Wireless Networking in the Developing World](http://wndw.net/) — Libro libre sobre diseño, implementación y mantenimiento de redes wifi de bajo costo. El capítulo 8 está dedicado a mesh.
- [open80211s HOWTO](https://github.com/o11s/open80211s/wiki/HOWTO) — Introducción rápida y guía paso a paso para montar una red mesh con open80211s.
- [Coolab Wiki — Aplicativos e serviços para redes locais](https://wiki.coolab.org/index.php/Aplicativos_e_servi%C3%A7os_para_redes_locais) (PT) — Más recursos en portugués.

## Protocolos de mesh

### Routing

- [Babel / babeld](https://www.irif.fr/~jch/software/babel/) — Protocolo de routing distance-vector loop-avoiding para IPv6/IPv4 con convergencia rápida; pensado para redes cableadas y wireless mesh. [`MIT`] [`C`] · [Código](https://github.com/jech/babeld)
- [B.A.T.M.A.N.-adv](https://www.open-mesh.org/projects/batman-adv/wiki) — Routing mesh que opera por debajo de IP, integrado en el kernel de Linux. [`GPLv2`] [`C`]
- [cjdns](https://github.com/cjdelisle/cjdns) — Red IPv6 cifrada que usa criptografía de clave pública para asignación de direcciones y una DHT para routing. [`GPLv3`]
- [GNUnet](https://gnunet.org/) — Capa de routing mesh con cifrado end-to-end y framework para apps distribuidas; busca reemplazar la pila insegura del Internet clásico. [`GPLv3`]
- [OLSR / OLSRd2](http://olsr.org/) — Optimized Link State Routing Protocol, IP routing optimizado para redes ad-hoc móviles y wireless. [`BSD`] [`C`] · [Código](https://github.com/OLSR/OONF)

### Stack

- [BLEMP](https://github.com/aanon4/BLEMP) — Bluetooth Low Energy Mesh Protocol para chips nRF51 de Nordic. [`BSD`] [`C`]
- [FruityMesh](https://github.com/mwaylabs/fruitymesh/wiki) — La primera mesh open-source completamente connection-based sobre BLE 4.1. [`GPLv3`] [`C++`]
- [Mesh Bee](https://github.com/Seeed-Studio/Mesh_Bee) — Módulo RF wireless 2.4 GHz basado en NXP JN516x para mesh ZigBee Pro. [`MIT`] [`C`]

## Firmware y sistemas para routers

- [LibreMesh](https://libremesh.org/) — Framework modular para crear firmwares basados en OpenWrt para nodos mesh wireless. Base de muchas redes comunitarias. [`AGPLv3`] [`Lua`] · [Código](https://github.com/libremesh/)
- [Quick Mesh Project (qMp)](https://qmp.cat/Home) — Sistema para desplegar redes mesh/MANET fácilmente sobre wifi. [`GPLv2`] [`C`] · [Código](http://dev.qmp.cat/projects/qmp/repository)
- [OpenWISP](https://openwisp.org/) — Sistema de gestión de redes hackeable para el siglo XXI; para administrar grandes despliegues de nodos. [`GPLv3`]

## Sistemas operativos para self-hosting

- [YunoHost](https://yunohost.org/) — Sistema operativo basado en Debian para alojar fácilmente múltiples servicios de intranet. [`AGPLv3`]
- [UBOS](https://ubos.net/) — Distro Linux que apunta a hacer 10× más fácil el self-hosting de aplicaciones web populares. [`AGPLv3`]

## Hardware mesh y offgrid

- [Disaster Radio](https://disaster.radio/) — Red de comunicaciones resiliente a desastres alimentada por sol; hardware + firmware + apps. [`GPLv3`] · [Código](https://github.com/sudomesh/disaster-radio/)
- [Meshtastic](https://meshtastic.org/) — Comunicador GPS mesh open-source y hackeable para senderismo, vuelo, ski y comunicación segura, basado en LoRa. [`GPLv3`]
- [LibreRouter](https://librerouter.org/) — Hardware libre para nodos de redes comunitarias (mencionado en MonteLibre como complemento a LibreMesh).

## Software all-in-one para mesh

- [LifeNet](http://thelifenetwork.org/about.html) — Solución de comunicación de datos por wifi diseñada para escenarios post-desastre; corre en laptops, smartphones y routers comunes. [`GPLv3`] [`C`] · [Código](https://github.com/hrushim/LifeNet)
- [Commotion Wireless](https://commotionwireless.net/) — Herramienta open-source que crea redes mesh descentralizadas sobre routers, móviles y desktops. [`GPLv3`] [`C`] · [Código](https://github.com/opentechinstitute) — *Nota: proyecto histórico, escaso mantenimiento desde ~2017.*
- [Project Byzantium](http://project-byzantium.org/) — Mesh wireless ad-hoc para "el apocalipsis zombie": no requiere equipo especial, solo una PC x86 con interfaz wifi 802.11. [`GPLv3`] · [Código](https://github.com/Byzantium/Byzantium)

## Comunicación — mensajería y VoIP

- [Briar](https://briarproject.org/) — App de mensajería para activistas, periodistas y quien necesite comunicarse de forma segura y robusta. Sin servidor central; sincroniza por Bluetooth/Wi-Fi si Internet está caído, o por Tor si está activo. [`GPLv3`] [`Java`] · [Código](https://code.briarproject.org/akwizgran/briar)
- [Bitmask](https://bitmask.net/es) — App open-source para comunicaciones cifradas vía VPN, fáciles y seguras. [`GPLv3`]
- [Retroshare](https://retroshare.cc/) — Establece conexiones cifradas entre amigos y ofrece foros, canales, chat y mail descentralizados. Diseñado para máxima seguridad y anonimato. [`GPLv2+`]
- [Jami](https://jami.net/) — Videollamadas peer-to-peer, sin servidor central. [`GPLv3`]
- [Mumble](https://www.mumble.info/) — Chat de voz open-source de baja latencia y alta calidad. *Nota: el enlace original `mumble.com` es de un servicio comercial; el proyecto FOSS oficial vive en `mumble.info`.* [`BSD`]
- [KouChat](https://www.kouchat.net/) — Chat LAN serverless open-source para escritorio y Android. [`LGPLv3`]
- [Meshenger](https://github.com/meshenger-app/meshenger-android) — Llamadas P2P de audio/video sobre redes locales. Sin servidor ni Internet. [`GPLv3`]
- [Serval Mesh / Batphone](http://www.servalproject.org/) — Sistema de telecomunicaciones entre teléfonos móviles que funciona fuera del rango de torres celulares vía wifi. [`GPLv3`] [`Java`] · [Código](https://github.com/servalproject/batphone) — *Nota: desarrollo en pausa hace varios años.*
- [Splinternet](https://github.com/megamattron/SplinterNet) — Sistema de mensajería serverless e inbloqueable para Android. [`MIT`(?)] [`Java`]
- [AirChat](https://github.com/lulzlabs/AirChat) — Comunicaciones libres por radio: cada nodo solo escucha lo que recibe, sin identificación de hardware ni de transmisor. [`modified-WTFPL`] [`Perl`]
- [Underdark](http://underdark.io/) — Librería mesh P2P móvil para iOS y Android sobre Wi-Fi y Bluetooth. [`Apache 2.0 modificada`] [`Java`] · [Código](https://github.com/udark/underdark-android)

## Comunicación — redes sociales y P2P

- [Manyverse](https://www.manyver.se/) — Red social sin las cosas malas, construida sobre el protocolo P2P Scuttlebutt (SSB). Para escritorio y móvil. [`MPL-2.0`]
- [Elgg](https://elgg.org/) — Motor de redes sociales open-source premiado, base flexible para construir todo tipo de entornos sociales. [`GPLv2 / MIT`]

## Videollamadas y streaming

- [Jitsi Meet](https://meet.jit.si/) — Plataforma de videollamadas que opera desde el navegador, sin instalación. [`Apache 2.0`]
- [VDO.Ninja](https://vdo.ninja/) — Lleva video en vivo desde un smartphone o computadora remota a OBS u otro software de estudio vía WebRTC P2P. Sin descargas, sin login, sin recolección de datos. [`AGPLv3`] (mostly open-source, ver [LICENCE.md](https://github.com/steveseguin/vdo.ninja/blob/develop/LICENCE.md))

## Multimedia

- [Jellyfin](https://jellyfin.org/) — Solución multimedia construida por voluntarios; stream a cualquier dispositivo desde tu propio servidor. [`GPLv2`]
- [Ampache](https://ampache.org/) — Aplicación web de streaming de audio/video y manejo de archivos accesible desde cualquier dispositivo con Internet. [`AGPLv3`]
- [MediaGoblin](https://mediagoblin.org/) — Plataforma libre de publicación multimedia descentralizada; alternativa a Flickr, YouTube, SoundCloud, etc. [`AGPLv3`]

## Productividad y colaboración

- [Nextcloud](https://nextcloud.com/) — Plataforma de productividad self-hosted que te mantiene en control de tus datos. [`AGPLv3`]
- [HedgeDoc](https://hedgedoc.org/) — Editor markdown colaborativo open-source, web-based, self-hosted, en tiempo real. [`AGPLv3`]
- [Etherpad](https://etherpad.org/) — Editor online open-source altamente customizable con edición colaborativa en tiempo real. [`Apache 2.0`]
- [Mattermost](https://mattermost.com/) — Plataforma open-source para colaboración de developers; alternativa a Slack. *Nota: open-core — Team Edition es FOSS (`MIT/AGPLv3`), Enterprise Edition es comercial.*

## Educación offline

- [Kolibri](https://learningequality.org/kolibri/) — Conjunto adaptable de soluciones abiertas para educación; plataforma offline-first para dispositivos de bajo costo. [`MIT`]
- [Internet-in-a-Box](https://internet-in-a-box.org/) — Instala recursos educativos como Wikipedia, Maps y Moodle en una Raspberry Pi como hotspot. [`GPLv2`]
- [Kiwix](https://www.kiwix.org/) — Lector offline para contenido como Wikipedia, Project Gutenberg o TED Talks. Software y contenido libres. [`GPLv3`]
- [KA Lite](https://ka-lite.readthedocs.io/) — App Django ligera para servir el contenido core de Khan Academy desde un servidor local, con tracking de puntos y progreso. [`MIT`] — *Nota: proyecto descontinuado oficialmente; reemplazado por Kolibri.*
- [PirateBox](https://piratebox.cc/) — Sistema DIY anónimo y offline de compartición de archivos y comunicaciones. [`GPLv3`] — *Nota: proyecto descontinuado en 2022; el código sigue disponible.*

## Mapas

- [uMap](https://umap.openstreetmap.fr/es/) — Crea mapas con capas de OpenStreetMap en un minuto y embébelos en tu sitio. [`WTFPL`]

## Seguridad y privacidad

- [Pi-hole](https://pi-hole.net/) — Servidor DNS abierto que bloquea publicidad antes de descargarla. [`EUPL-1.2`]

## Software P2P / descentralizado (extras de awesome-mesh)

- [Freenet](https://freenetproject.org/) — Red de nodos cuyas comunicaciones se enrutan cifradas a través de otros nodos, dificultando saber quién pide qué. [`GPLv2`] [`Java`] · [Código](https://github.com/freenet/fred)
- [IPFS (Go-IPFS / Kubo)](https://ipfs.io/) — Sistema de archivos P2P versionado y global; combina ideas de Git, BitTorrent, Kademlia, SFS y la Web. [`MIT/Apache-2.0`] [`Go`] · [Código](https://github.com/ipfs/kubo)
- [ZeroNet](https://zeronet.io/) — Red descentralizada P2P tipo Internet; cada visitante es también host. [`GPLv2`] [`Python`] · [Código](https://github.com/HelloZeroNet/ZeroNet) — *Nota: desarrollo principal con poco movimiento; existe el fork activo `ZeroNet-Conservancy`.*

## Comunidades

### Online

- [DarkNetPlan](https://www.reddit.com/r/darknetplan/) — Comunidad de Reddit sobre comunicaciones offgrid y mesh.
- [Hyperboria](https://hyperboria.net/) — Comunidad de iniciativas wifi locales, programadores y entusiastas. La mayor red pública cjdns.
- [MeshLocals](https://github.com/phillymesh/meshlocals/blob/master/meshlocals.md) — Lista de todos los meshlocals trabajando en redes mesh.

### Offline / encuentros

- [Battle of the Mesh](http://battlemesh.org/) — Torneo europeo con carácter social para entusiastas de mesh y activistas de redes comunitarias.
- [Broadband-Hamnet / AREDN](https://www.arednmesh.org/) — Red wireless de alta velocidad, autoconfigurable y tolerante a fallos; foco en comunicaciones de emergencia para radioaficionados.
- [Freifunk](https://freifunk.net/en/) — El proyecto comunitario de wifi más grande de Alemania.
- [Guifi.net](https://guifi.net/en) — El proyecto comunitario de wifi más grande de España.
- [SudoRoom Mesh](https://sudoroom.org/wiki/Mesh) — Colectivo de Oakland, California que lleva años trabajando en mesh.
- [AlterMundi](https://altermundi.net/) — Red de organizaciones latinoamericanas que promueven redes comunitarias (vinculada a LibreMesh y LibreRouter).
- [MonteLibre](https://montelibre.net/) — Red comunitaria en Argentina; fuente original de parte de esta lista.

## Recursos adicionales

- [MonteLibre — Aprendiendo sobre Redes Mesh](https://montelibre.net/blog/aprendiendo-sobre-redes-mesh/)
- [MonteLibre — Potencia TX y Canales por Países](https://montelibre.net/blog/potencia-tx-y-canales-por-paises/)
- [MonteLibre — Compilando LibreRouterOS para TpLink CPE510 v3](https://montelibre.net/blog/compilando-librerouteros-para-tplink-cpe510-v3/)

---

## No-código-abierto / source-available

Esta sección lista proyectos mencionados en las fuentes originales que **no son software libre/open-source completo**, ya sea porque son servicios alojados, freeware propietario, o tienen un modelo open-core con componentes propietarios significativos. Se incluyen porque pueden ser útiles en contextos de redes comunitarias y offgrid, pero conviene saber su estatus legal.

- **[meet.jit.si](https://meet.jit.si/)** — *Servicio alojado (no software).* El software [Jitsi Meet](https://github.com/jitsi/jitsi-meet) sí es Apache 2.0 y figura arriba; pero `meet.jit.si` como servicio operado por 8x8 no es código en sí mismo, sino una instancia gestionada por una empresa.
- **[Mumble.com](https://www.mumble.com/)** — La URL original de la entrada de MonteLibre apunta a un servicio/marca comercial, no al proyecto FOSS. El proyecto libre Mumble (BSD) está en [mumble.info](https://www.mumble.info/) y figura arriba.
- **Mattermost Enterprise Edition** — La edición empresarial de Mattermost es propietaria (licencia comercial). Solo el Team Edition / código del repositorio principal es FOSS bajo MIT/AGPLv3 (ya listado arriba).

> Nota: en el listado original de MonteLibre **todos los proyectos son declarados como open-source o software libre**, y la lista de awesome-mesh está explícitamente restringida a "Free Software". La sección de arriba captura los matices y casos borde más que verdaderos proyectos cerrados.

---

## Licencia

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

Esta lista está dedicada al dominio público bajo CC0. Las listas originales tienen sus propias licencias:

- [moarpepes/awesome-mesh](https://github.com/moarpepes/awesome-mesh) — CC BY-SA 3.0
- [MonteLibre](https://montelibre.net/) — ver el sitio para condiciones.

## Contribuir

Pull requests bienvenidos. Por favor mantené el formato (nombre — descripción breve — `[licencia]` · enlace al código si aplica) y verificá que el proyecto siga vivo o señalá si está descontinuado.
