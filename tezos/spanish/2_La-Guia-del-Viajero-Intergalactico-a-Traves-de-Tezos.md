# La Guía del Viajero Intergaláctico a Través de Tezos
Awa Sun Yin, Sep 19, 2018
El propósito de este artículo es brindar al lector los elementos más esenciales que uno debe saber sobre Tezos, si no se tiene un conocimiento previo sobre esta plataforma, de manera tal que los lectores que interactúan con la red, o planean hacerlo, podrán lograrlo bien informados y con la comprensión requerida.
Los tópicos cubiertos en este artículo abarcan desde una introducción al protocolo Tezos, a tópicos económicos para “panaderos” (bakers) y “delegantes”(delegators).
Nota: este artículo es estrictamente sobre Tezos como proyecto y ecosistema. Por esta razón, no planeamos ahondar en las historias detrás del proceso de fundación o la controversia que el proyecto ha sufrido. Para más información, lea el artículo de WIRED.

## ¿Qué es Tezos?
Tezos es un legajo público distribuido, o una cadena de bloques, un proyecto de fuente abierta, mayormente desarrollado en OCaml, un lenguaje de programación funcional. Además del legajo, es una plataforma de contratos inteligentes que brinda soporte a contratos desarrollados en un lenguaje llamado Michelson. Michelson es un lenguaje de asignación rigurosa, como OCaml, optimizado para escribir contratos inteligentes que facilitan la verificación formal (métodos que pueden contribuir a la exactitud de los sistemas, útiles para por ejemplo, detectar vulnerabilidades tales como la infame DAO o la vulnerabilidad de la Multi-Sig Wallet). Michelson por diseño, está limitado a escribir aplicaciones relacionadas a las cadenas de bloques, como carteras “multi-sig”, otorgamientos, y reglas de distribución que apuntan a facilitar el chequeo de lo que se requiere ser ejecutado exactamente.
Además de la elección de los lenguajes de desarrollo, Tezos se caracteriza por tener su propia interpretación e implementación de Prueba de Participación (PoS), conocida como Prueba de Participación Líquida (LPoS), como un mecanismo para determinar las condiciones de los pares o nodos deben completar para participar del consenso. LPoS se utiliza en combinación con el Consenso Nakamoto, que indica que la cadena más larga es la canónica (correcta), para incentivar entidades para mantener la infraestructura y coordinar al mismo tiempo los partidos “trustless — sin necesidad de aval/confianza” que conforman la red Tezos.
Otro factor a resaltar, que el proyecto Tezos busca, es la gobernancia “en-cadena”. La gobernanza, en el mundo de la cadena de bloques, refiere al proceso o sistema para diseñar, proponer, reafirmar e implementar cambios a un protocolo o proyecto. El lema de Tezos “Tezos — un cripto-legajo autónomamente enmendado” se refiere al objetivo de Tezos de brindar soporte para modernizaciones o cambios no solo en el código fuente, si no también en el proceso de gobernancia, la aprobación o rechazo se determinan a través de un sistema de voto “en cadena” (dentro de la cadena de bloques Tezos).
La oferta de moneda inicial (ICO) de Tezos comenzó el 1ero de Julio de 2017, finalizando el 13 del mismo mes, recaudando $232 millones para 763,306,929.69 XTZ lo cual incluye un 20% de los tokens en contratos emplazados, según este estudio estadístico del evento.A pesar de ser una iniciativa de fuente abierta, significando esto que cualquier individuo puede contribuir al código fuente, la mayoría del proyecto se encuentra siendo desarrollado, llevado a producción y mantenido por una entidad basada en Delaware llamada Dynamic Ledger Solutionsy el equipo OCamlPro, una compañía Francesa de desarrollo web.
Actualmente, hay tres principales versiones de software de Tezos: zeronet, alphanet, y betanet. Estas son, respectivamente: una “testnet” que incluye elementos más experimentales y orientados al desarrollo; una “testnet” con los elementos estables más recientes, y la testnet que se encuentra más cerca a producción, en la cual transacciones y originaciones (contratos inteligentes) persistirán en la mainnet. El lanzamiento de la mainnet (conocido como “cita para el almuerzo”) tuvo lugar el 17 de Septiembre, acorde a la Fundación Tezos. La transición de betanet a mainnet implica un cambio del cambio de etiquetas. La betanet fue lanzada el 3o de Junio de 2018, y operada por 8 “panaderos” Tezos hasta el ciclo 7. En el ciclo de escritura (ciclo 26), se pueden identificar 411 panaderos distintos.

### Particularidades del protocolo Tezos a conocer
El tiempo se mide en Ciclos (~2–3 días). Existen dos tipos de cuentas: unas que comienzan con TZ1 que contienen los fondos, y otras comenzando con KT1 que forman las originaciones (contratos inteligentes) para la delegación. Tezos es una cadena de bloques pública, cualquiera que complete los requerimientos de propia garantía (10,000 XTZ como Prueba de Participación) puede participar del consenso.Antes del lanzamiento de la mainnet, había sólo tres maneras de adquirir XTZ: habiendo participado de la venta pública (para usar esos fondos uno tiene que pasar por un KYC (CSC) para activar la cuenta), o bien comprar en los portales de cambio Coinone o Gate.io, o en derivados OTC (entre pares, sin regulación).
Nota: desde el lanzamiento a mainnet, han habido nuevos portales que ahora brindan servicios de cambio para XTZ.

## Depositarios/interesados mayores en Tezos

### La Fundación
La Fundación Tezos es una entidad sin fines de lucro fundada en Zug y regulada por las leyes suizas. La Fundación tiene como mandato la promoción y el desarrollo de tecnologías y aplicaciones, en particular, arquitecturas abiertas y descentralizadas, con foco en (pero no limitadas a) el Protocolo Tezos. El texto original (en Alemán), explica lo siguiente:
Förderung und Entwicklung von neuen Technologien und Applikationen, insbesondere in den Bereichen von neuen offenen und dezentralisierten Softwarearchitekturen; im Vordergrund — aber nicht ausschliesslich — steht dabei die Förderung und Entwicklung des so genannten Tezos Protokolls und der entsprechenden Technologien, sowie die Förderung und Unterstützung von Applikationen unter Anwendung des Tezos Protokolls; vollständige Zweckumschreibung gemäss Statuten — El propósito de la Tezos Stiftung, como quedó asentado en el registro comercial del Cantón de Zug.
Para cumplir con este propósito, la Fundación lanzó un programa de becas dedicado a la investigación, desarrollo, y esfuerzos comunitarios (tales como nosotros, Cryptium Labs)

### Dynamic Ledger Solutions
Dynamic Ledger Solutions es la entidad dedicada a desarrollar y lanzar la red Tezos. A cambio, la Fundación Tezos le brindará 8,5% de los fondos de la venta pública además de un 10% de los tokens originados en el proceso de Génesis como remuneración.
Poseedores de XTZ
Las entidades que hayan comprado XTZ en la venta pública en los portales de cambio Coinone o Gate.io, o en derivados OTC (entre pares, sin regulación). Los poseedores pueden naturalmente utilizar los fondos para propósitos múltiples, entre los cuales se encuentran los más comunes: transferencia, bonding (ver “panaderos”), delegar (ver “delegantes/delegators”), donaciones (a por ejemplo, proyectos de fuente abierta) o simplemente mantenerlos en sus cuentas (“hodling”). La última opción no es recomendada ya que “mantener” estos tokens diluye lentamente su valor relativo debido a la inflación(~5.51% del total por año, distribuido sólo a los panaderos y delegantes/delegators).

### Panaderos (Validadores)
Las entidades que han asignado una suma mínima de XTZ de propia garantía (participando en la red), los convierte en elegibles para participar en el consenso y así poder recibir “baking” (hornear)(validación de bloques, ingresos (16 XTZ + comisión por transferencias incluidas en el bloque) y recompensas por aprobaciones (endorsements) (ganando 1 o 2 XTZ por aprobación). A pesar que existen individuos actuando como panaderos (también conocidos como solo-baking), hay entidades que brindan servicios públicos a los poseedores del token a cambio de comisiones de servicio. Esto significa que por cada “bloque horneado”, el suministro total de XTZ se incrementa por 16 XTZ.
Más lecturas (en inglés por el momento) — Is Your Favourite Baker Overdelegated? Understanding Self-Bond Requirements in Tezos: https://medium.com/cryptium/is-your-favourite-baker-overdelegated-understanding-self-bond-requirements-in-tezos-bb005a05c609
El “horneado” o baking y los derechos de aprobación son asignados a aquellos panaderos que siguen un sistema similar a una lotería, con listas de prioridad. Debido a esto, los panaderos senior podrán ganar hasta el momento mayores sumas de recompensas, a diferencia de nuevos panaderos, debido a que el número de panaderos, en este momento, se incrementa ciclo a ciclo.
La (pseudo) randomización de asignación de lugares es generada por un sistema de multi-pasos y la combinación de diferentes valores, tales como generación de seeds randomizadas consistiendo de un número de 256 bit generado al final de un ciclo X, los compromisos realizados en el ciclo anterior, hasta 32 revelaciones, y por medio de hashing de todas las revelaciones. Han habido rumores acerca de Tezos cambiando a Compartición Pública Verificable de Secretos (por ejemplo, Shamir’s Secret Sharing) para la generación de la randomización.
Leer más (en Inglés por el momento) — Introduction to Proof-of-Stake in Tezos and Understanding Baking and Endorsement Rewards: https://medium.com/cryptium/hello-admin-when-payout-tez-19fc5e460cce
Los panaderos públicos no se pueden negar a las delegaciones, que son originaciones en-cadena (contratos inteligentes) y deben asignar de propia garantía un mínimo dependiendo de la total suma de delegación que recibieron. Cuando la garantía no cubre la totalidad de la delegación, el panadero se encuentra “sobredelegado” (overdelegated). La única medida de evitar esto es no pagar las recompensas correspondientes a la suma que causó la sobredelegación, y así los delegantes(delegators)son desalentados de hacer esto.
Las recompensas por protocolo son pagadas a la dirección del panadero. Esto significa que hay una relación de confianza entre los panaderos y sus delegados, debido a que el anteriormente mencionado debe confiar que el anterior le pague las recompensas profesionales a los delegados correspondientes.
Los panaderos pueden perder al menos 512 XTZ (más las recompensas ganadas al momento) por cada bloque con doble firma, y un máximo de su garantía total. Cuando los panaderos son penalizados, los tokens “se queman”, desapareciendo del suministro total. Sin embargo, el “double-baking” y doble-endoso (o aprobación) no afectan la probabilidad de ser asignados futuros lugares. Los panaderos que no han estado en línea al momento del “baking” o aprobación perderán su ingreso correspondientes, pero otros panaderos podrán ganar en su lugar (también llamado stolen blocks).

### Delegantes / Delegators (Delegación)
Los delegantes(delegators)son entidades que poseen XTZ y deciden delegar sus tokens a un panadero (o a sí mismos). Los delegantes (delegators) podrían, en teoría, ganar la suma proporcional a la delegación proporcional de las recompensas totales que un panadero ha producido. A cambio, los panaderos pueden decidir tomar una cuota deservicio.
Las delegaciones, en contraste con las transacciones, no causen al delegante (delegator) la pérdida de la custodia de sus fondos. Una delegación es una originación (un contrato inteligente) cuyo dueño es el anteriormente mencionado delegante (delegator). Entre otras cosas, la originación contiene un parámetro que es la dirección del panadero-objetivo, la cual es utilizada para asignar la delegación al panadero específico (nuevamente, esto no significa que el panadero podrá tomar control de los fondos).
A diferencia de la propia garantía de los panaderos, las delegaciones no pueden ser perdidas a modo de castigo por el double-baking o doble-endoso/aprobación del panadero. El mayor riesgo para los delegantes (delegators) es el costo de la oportunidad de delegar a un panadero que cierre el servicio. En este escenario, si una delegación no se cambia dentro del mismo ciclo, los fondos serán improductivos por un ciclo más, además de los 7 ciclos base (requeridos hasta que la delegación se tenga en cuenta en la nueva tanda de baking y plazas para aprobación/endose[9] [10] [SYH11] ). Otro riesgo considerable es la posibilidad de que un panadero no pague las recompensas o la posibilidad que un panadero no se encuentre activo para el baking asignado y plazas de aprobación/endose, causando la pérdida de las recompensas.
Leer más (en inglés) — Introduction to Proof-of-Stake in Tezos and Understanding Baking and Endorsement Rewards: https://medium.com/cryptium/hello-admin-when-payout-tez-19fc5e460cce

### El Ecosistema Tezos
Billeteras/carteras
Las billeteras/carteras son software que permite que los usuarios interactúan directa o indirectamente con la cadena de bloques. Existen dos tipos de carteras/billeteras, frías o hardware, y en línea, también conocidas como calientes. Las carteras y sus desarrolladores tienen un rol esencial en el ecosistema de las cadenas de bloques, ya que el uso de los tokens depende mucho de ellos. Una particularidad de las carteras en redes de Prueba de Participación (PoS) que las redes tradicionales como Bitcoin no tenían, es el soporte para delegación y de-delegación.
Los panaderos y desarrolladores normalmente utilizan el Cliente-Tezos que es una cartera basada en línea de comandos. Para obtener el Tezos-Client, uno debe instalar Tezos en su dispositivo. Esta línea de comando soporta acciones tales como la transferencia de fondos o generación de originaciones.
Lectura adicional (en inglés) — Guide to Installing and Delegating with Tezos-Client: https://medium.com/cryptium/how-to-delegate-tezos-xtz-with-tezos-client-and-running-your-own-node-betanet-cea6960cf45
Ledger Nano S es una cartera hardware o fría muy popular que brinda soporte a interacciones con el Tezos-Client. Para transferir fondos o hacer originaciones, uno debe aun interactuar con las herramientas de la línea de comandos, pero manteniendo los fondos en la cartera hardware aumenta la seguridad y es recomendado para grandes cantidades de tokens,
Han habido anuncios sobre Trezor, otra cartera hardware popular, brindando soporte a Tezos. El mayor riesgo con las carteras hardware tiene que ver con la compra de las mismas “usadas”, vengan de parte de proveedores oficiales o no, lo que implica que otra persona puede haber hecho un back-up de las palabras origen y podrá tener acceso a los fondos que se encuentran en la cartera.
Más lectura (inglés) — Guide to Delegate with Ledger Nano S: https://medium.com/cryptium/how-to-delegate-tezzies-tezos-xtz-with-your-ledger-nano-s-with-initial-setup-screenshots-519c9ae6654f
En el ecosistema Tezos, hay carteras “calientes” populares, desarrolladas por Stephen Andrew y el equipo Cryptoeconomic: TezBox Wallety Galleon Wallet (Cryptonomic). A medida que la comunidad Tezos crece, hay mas y mas esfuerzos de desarrollo invertidos en la usabilidad del protocolo. Aquí pueden encontrar una lista hecha por la comunidad de las carteras Tezos. Existen esfuerzos de desarrollo provenientes de todos los rincones del globo, por ejemplo, WeTez, basados en China.
Leer más (inglés) — Guide to Delegate with TezBox: https://medium.com/cryptium/how-to-delegate-tezos-xtz-with-tezbox-online-wallet-96592e94e357
Leer más (inglés) — Guide to Delegate with Galleon: https://medium.com/cryptium/how-to-delegate-tezos-xtz-with-galleon-wallet-7bdc44e954a8
Servicios esenciales
Más allá de los esfuerzos de desarrollo de protocolo y de carteras, existen equipos que brindan servicios esenciales para todo usuario o parte interesada en el ecosistema Tezos.
Los servicios exploradores de bloque son servicios gratis que funcionan como fuente de verdad basada en datos. Estos solicitan datos directamente de los nodos completos y son comúnmente utilizados para chequear si una transacción ha sido incluida en el siguiente bloque, para verificar en qué ciclo nos encontramos, o chequear los panaderos que están activos y estadísticas relacionadas con sus “bakings”, además de estadísticas genéricas sobre la red (suministro de tokens total o la cantidad global de propia garantía — self-bonded tokens). El explorador de bloques más popular es TzScan desarrollador por el equipo OCamlPro.
Debido a que los poseedores de tokens necesitan confiar a los servicios de baking en una cierta medida, los listados de baking son otro elemento de los servicios en ecosistemas de Prueba de Participación (PoS). Estos forman listas de los servicios de baking públicos y muestran métricas de cada uno de ellos, facilitando el descubrimiento de servicios y poder encontrar más información sobre ellos antes de delegar. Algunos listados populares de bakers son: MyTezosBaker, Tezos Rocks, oTzScan. ¡Podemos encontrar, incluso, servicios que brindan la proporción de bakings y endorsements de éxito de los panaderos, como Bakendorse!
Comunidad

## Créditos
Artículo original (Inglés): https://medium.com/cryptium/the-hitchhikers-guide-to-tezos-36f112662074
Nota: La versión actual se ha escrito en español neutro para facilitar la lectura a diversas communidades hispano-hablantes alrededor del mundo.
Traducción al español: Maria Paula Fernández