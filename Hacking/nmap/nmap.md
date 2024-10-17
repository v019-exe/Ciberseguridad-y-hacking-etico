# NMAP (Network Mapper)

1. Reconocimiento activo (Fingerprinting): Interacción directa con el objetivo, es ilegal sin autorización
2. Reconocimiento pasivo (Footprinting): Recopilación de información, sin interacción directa con el objetivo. Es legal


Tiene una base de datos que se llama Nmap Services

Arquitectura, modular

NSE (Nmap Scripting Engine), Scripts de NMAP añaden funcionalidades a NMAP

## ESTADOS
1. Abierto (Open)
2. Cerrado (Closed)
3. Filtered (Filtrado)
4. Unfiltered (No filtrado)
5. Open | Filtered (Abierto | Filtrado)
6. Closed | Filtered (Closed | Filtered)

### TCP
Principales estados

1. Abierto: Puerto abierto tipo escaneo TCP/SYN es cuando devuelve un SYN/ACK, finaliza con un segmento RST (RESET), RST evita que termine el handshake y nos puedan detectar.
2. Cerrado: Envia segmento SYN y recibe RST lo que significa que ele peurto está cerrado, es accesible pero no responde ningún servicio
3. Filtrado: Envia el segmento SYN pero no recibe respuesta, normalmente pasa cuando hay un firewall delante.
4. No filtrado: Llegan al destino pero no puede determinar si el puerto está abierto o cerrado. Ocurre cuando no se usa TCP/SYN

### UDP
Principales estados
1. Abierto: NMAP envía un datagrama UDP y recibe una respuesta de la aplicación. Significa que está abierto.
2. Cerrado: Envía un datagrama UDP y recibe una respuesta de tipo ICMP (Port Unreachable), significa que está cerrado.
3. Abierto Filtrado: Envía un datagrama UDP, pero no puede determinar si está abierto o no por qué no responde al datagrana UDP.
4. Filtrado: No recibe respuesta al datagrama UDP, después de varios intentos

IP ID IDLE, con un zombie, este ataque no revela la IP del atacante.



## TIPOS DE ESCANEOS NMAP
1. TCP
2. TCP/SYN
3. ACK
4. FIN
5. NULL
6. MAIMON


# NMAP CLI
nmap recibe argumentos, parámetros "Subparámetros (De los parámetros pueden salir mas parámetros)"

Si nmap se ejecuta sin permisos de root hará escaneo TCP, con root se hace escaneo TCP/SYN por defecto.

Especificaciones:
1. Directa: nmap <ip>
2. Especificación desde lista: -iL sirve para pasarle un archivo de texto con IPs 
3. Exclusiones: decirle a nmap que no escanee unas direcciones IP, parámetro --exclude, --excludefile (Excluye las direcciones IP de un archivo)

## GESTIÓN DE PUERTOS
Todo esto es TCP/SYN, Parámetro básico *-p*, de puerto

Dentro de -p podemos usar los protocolos:
T: TCP
U: UDP

Otros parámetros:
1. -sU (UDP)
2. -sT (TCP, conexión completa)
3. -p- (Todos los puertos)
4. --exclude-ports (Sirve para excluir puertos)
5. --top-ports (Escanea los puertos mas comunes, toma como argumento 1 numero)
6. -sS (Escaneo tipo SYN)
7. --port-ratio (Puertos mas usuados con umbral de frecuencia), toma porcentajes ejemplo 10% (0.1)

Se puede especificar en rango, separado por comas o individalmente
1. nmap -pU:9999, T:22, 80 <ip>
2. nmap -p 1:65535 <ip>
3. nmap -p 22 <ip>

## ESCANEOS TCP
Primero de todo, no es lo mismo que TCP/SYN

Primeramente sigue la estructura SYN - ACK / ACK - ACK

Orden de conexión

1. SYN (Cliente)
2. SYN-ACK (Servidor)
3. ACK (Cliente)

Hay que tener cuidado con los firewalls, si hay firewalls con reglas estrictas puede ser que este tipo de conexiones las bloquee.

## ESCANEOS TCP/SYN

Primeramente este se diferencia por una cosa:

1. SYN (Cliente o atacante)
2. SYN/ACK (Víctima)
3. RST

## ESCANEOS UDP CON NMAP

Parámetros de verbosidad
1. -vvv

Los escaneos udp son exageradamente mas lentos que un escaneo TCP o TCP/SYN

Parámetro -sU para escaneo de puertos UDP pero todos los puertos

## Escaneos SCTP con NMAP

SCTP = Stream Transmission Control Protocol (SCTP) Capa 4

Parámetros: 
1. -sY (Similar a -sS, envía un paquete SCTP INIT al puerto que se escanea, responde INIT-ACK si está abierto. ABORT si está cerrado)
2. -sZ (Continuación de la conexión, INIT, INIT-ACK, COOKIE-ECHO (Procede a conectarse))

## Escaneos FIN

Este escaneo se hace con el parámetro -sF

Puertos abiertos enviando paquetes FIN no responden
Puertos cerrados envían como respuesta RST

## ESCANEOS NULL
Este escaneo se hace con el parámetro -sN


Puertos abiertos enviando paquetes NULL no responden
Puertos cerrados envían como respuesta RST

## ESCANEOS XMAS

Este escaneo se hace con el parámetro -sX

Este escaneo el paquete va con 3 flags
FIN
PSH (PUSH)
URG (URGENTE)

Son paquetes "Iluminados"

Si el puerto está cerrado responde con RST
y si está abierto puede ser que responda o no responda

## ESCANEOS MAIMON

Este escaneo se hace con el parámetro -sM

Puertos abiertos enviando paquetes FIN-ACK no responden
Puertos cerrados envían como respuesta RST


## DESCUBRIR S.O
Para descubrir un sistema operativo se usa el parámetro -O

Parámetros extra:
1. --osscan-limit
2. --osscan-guess (MODO AGRESIVO PARA DETECTAR EL SISTEMA OPERATIVO)

## VELOCIDAD Y TRÁFICO DE LOS ESCANEOS

Parámetros:
1. -T (del 0 al 5 toma como argumento), 0 es enviar peticiones como una abuela y 5 es una abuelita con esteroides xd

0 es Paranoid (Sigiloso)
1 Sneaky (Algo mas rápido que paranoid)
2 Polite (Algo mas rápido pero prioriza no ser detectado)
3 normal (Por defecto)
4 Agresivo (Envía mas peticiones, riesgo de ser detectado.)
5 Insane (Provoca mucho ruido en la red, muy alto riesgo de ser detectado, propenso a dar falsos positivos)

2. --host-timeout (Establece un límite de tiempo, por si el host no responde entonces abandona el escaneo tras x segundos, minutos, horas)

3. --min-rate (Control de tasa de paquetes enviados)
4. --max-rate (Toma como argumento valores númericos)

## ESCANEO + VERSIONES DE SERVICIOS

Para detectar versiones de servicios usamos el parámetro -sV

Dentro de -sV tenemos mas parámetros

1. --version-intensity (del 0 al 9)
0 Feto. (Ligero)
9 John Cena con esteroides

2. --version-light (--version-intensity al 2)
3. --version-all (--version-intensity al 9 (JOHN CENA CON ESTEROIDES))
4. --version-trace (Salida detallada de la actividad del escaneo)

## Formatos de salida CON EXPORTACIÓN

Formatos de salida

1. -oN (Formato normal)
2. -oG (Formato compatible con grep)
3. -oX (Formato XML)
4. -oS (Para script kiddies)
5. -oA (Exportar en todos los formatos)

## Formatos de salida sin exportación 

1. -v (verbosa hasta -vvv)
2. -d (depuración)
3. --reason (Por qué está abierto ese puerto)
4. --open (Muestra solo los puertos que nmap consideró abiertos)
5. --packet-trace (Muestra el tráfico de los paquetes)

## HOST DISCOVERY

Hostdiscovery trata de enviar paquetes con todas las flags activadas

Parámetros:
1. -sn (Sin sondeo de puertos, desactiva el escaner de puertos. Envia pings para descubrir hosts)
2. -Pn (Quita el descubrimiento de host, fuerza a que no intente ningun tipo de descubrimiento)
3. -PS (Host discovery basado en TCP SYN)
4. -PA (Host discovery basado en TCP ACK)
5. -PU (Host discovery basado en UDP)
6. -PY (Host discovery basado en SCTP)

### BASADOS EN ICMP
Con estos parámetros le decimos a NMAP que use sondas de descubrimiento basadas en ICMP
1. -PE (ECHO REQUEST)
2. -PP (TIMESTAMP REQUEST)
3. -PM (SUBNET MASK ICMP (NETMASK REQUEST))

## HOST DISCOVERY II

1. -PO (permite especificar una lista de protocolos (TIPO PING))
**IANA PROTOCOLOS NUMEROS**
ICMP: 1
IGMP: 2
TCP: 6
EGP: 8
UDP: 17
IPv6: 41
ESP: 50
AH: 51
ICMPv6: 58
OSPF: 89
SCTP: 132

2. -n (No resolución DNS)
3. -R (Forzar al máximo la resolución DNS)
4. --dns-servers (Especificar servidores DNS)
5. --system-dns (Usará el DNS del sistema)
6. --traceroute (Ejecuta un traceroute)

## NSE TEORÍA

Escrito en LUA, añade funcionalidades a NMAP

Scripts:

1. Auth Scripts que prueban o eluden la autenticación en aplicaciones y protocolos
2. Broadcast: Scripts que descubren hosts enviando paquetes a direcciones de difusión.
3. Brute: Intentan fuerza bruta en cuentas de diferentes servicios.
4. Default: Scripts que se ejecutan por defecto junto con la detección de servicios
5. Discovery: Scripts utilizar para descubrir más información sobre la red, como identificar dispositivos y servicios.
6. DoS: Prueban si un host es vulnerable a ataques de denegación de servicio.
7. Exploit: Intentan "explotar" vulnerabilidades.
8. External: Scripts que interactuaran con activos en internet para su funcionamiento
9. Fuzzer: Envian entradas inesperadas o aleatorias a las aplicaciones para descubrir posibles fallos.
10. Intrusive: Scripts que se consideran intrusivos y pueden afectar al rendimiento o la estabilidad del sistema objetivo.
11. Malware: Buscan indicadores de sistemas operativos comprometidos o infectados.
12. Safe: Scripts que no son intrusivos y se consideran seguros para ejecutar en entornos de producción.
13. Version: mejoran la detección de versiones de Nmap o prueban versiones especificas de servicios para obtener información detallada.
14. Vuln: Scripts que permiten detectar vulnerabilidades en bvase de la información del escaneo.

Los scripts se almacenan en /usr/share/nmap/scripts

COMANDO FIND: find /usr/share/nmap/scripts -type f -name "*.nse" -print0 | xargs -0 grep 'categories' | grep 'vuln'

PARÁMETROS:

1. --script=<nombre script>
2. -sC (Ejecuta todos los scripts de la categoria default)
3. --script-args (Pasar argumentos a scripts)
4. --script-help (Argumento, nombre del script)
5. --script-trace (Muestra todos los datos enviados y recibidos)
6. --script-updatedb (Actualiza la base de datos)
7. -A (Mete varios argumentos en uno)