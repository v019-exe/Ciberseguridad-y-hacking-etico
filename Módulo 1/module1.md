# Ciberseguridad y ciberinteligencia

## Amenazas comunes

### Dominios de Amenazas

Se pueden aprovechar los sistemas dentro de un dominio mediante:
- Acceso directo y físico a sistemas y redes
- Redes inálambricas que se extiendnen mas allá de los límites de una org.
- Bluetooth o NFC
- Tipos de adjuntos maliciosos
- Elementos menos seguros dentro de la cadena de abastecimiento de una org
- Cuentas de medios sociales de una org.
- Medios extraíbles, unidades flash (USB)
- Aplicaciones basadas en la nube

## Tipos de amenazas cibernéticas

Podemos clasificarlas en diferentes categorias.

- Ataques de software
- Errores de software
- Sabotaje
- Error Humano
- Robo
- Fallas del hardware
- Interrupción de servicios
- Desastres naturales

## Amenazas internas vs externas

- Amenazas internas: generalmente son llevadas a cabo por empleados actuales o anteriores y otros socios contractuales que manipulan accidental o intencionalmente los datos confidenciales o amenazan las operaciones de servidores o dispositivos de infraestructura de red conectando medios infectados o accediendo a correos electronicos o sitios web maliciosos.

- Amenazas externas: Expertos pueden explotar vulnerabilidades en los dispositivos conectados a la red o pueden utilizar la ingeniería social, como trucos, para obtener acceso.

## vulnerabilidades
Un dominio de usuario incluye cualquier persona con acceso al sistema de información de una organización, incluidos empleados, clientes y partners contractuales.

- Sin conocimiento sobre seguridad
- Políticas de seguridad aplicadas de modo eficiente
- Robo de datos
- Descargas no autorizadas
- Redes privadas virtuales no autorizadas
- Sitios web no autorizados.
- Destrucción de sistemas, aplicaciones o datos.

## Amenazas
**CUALQUIER DISPOSITIVO QUE QUEDE ENCENDIDO Y DESATENDIDO REPRESENTA EL RIESGO DE QUE ALGUIEN OBTENGA ACCESO NO AUTORIZADO A LOS RECURSOS DE LA RED.**

**DESCARGA DE FICHEROS EXTRAÑOS**

Entre otros son las amenazas comunes que pueden vulnerar un dispositivo.

## Amenazas en la LAN
Podemos identificar diferentes ejemplos de amenazas a la LAN se incluyen:
- Acceso no autorizado a los centros de datos, salas de ordenadores y los armarios de cableado.
- Acceso no autorizado a los sistemas, aplicaciones y los datos.
- Acceso no autorizado de usuarios dudosos en las redes inálambricas
- Ataques a los datos en transito (MITM)
- Tener servidores LAN con hardware o sistemas operativos diferentes hace que administrarlos y solucionarlos sea mas difícil.
- Escaneo de puertos y sondeo de redes no autorizados.
- Cortafuegos mal configurado.

## Amenazas a la nube privada
El dominio de nube privada incluye servidores, recursos e infraestructura de TI privados disponibles para los miembros de la organización a través de Internet.

- Escaneo de puertos y sondeo de redes no autorizados
- Acceso no autorizado a los recursos
- Vulnerabilidad del software del sistema operativo de los dispositivos
- Error en la configuración del router, cortafuiegos o dispositivo de red
- Usuarios remotos que acceden a la infraestructura de la organización y descargan datos confidenciales.

## Amenazas a la nube pública
Cuando un dominio de nube privada aloja recursos de computación para una sola organización, el dominio de nube pública es la totalidad de los servicios de computación alojados por una nube, un servicio o un proveedor de Internet que están disponibles para el público y se comparten entre las organizaciones.

Tenemos 3 tipos:

- SaaS (SOFTWARE COMO SERVICIO): un modelo por suscripción que brinda acceso al software alojado de manera centralizada al qu los usuarios acceden mediante un navegador web.
- PaaS (PLATAFORMA COMO SERVICIO): proporciona una plataforma que permite que una org desarrolle, ejecute y administre sus apps en el hardware del servicio con herramientas provistas por el servicio.
- IaaS (INFRAESTRUCTURA COMO SERVICIO): proporciona recusos de computación virtualizados, como hardware, software, servidores, almacenamiento y otros componentes de infraestructura en Internet.

## Amenazas a las aplicaciones
El dominio de aplicación incluye todos los sistemas críticos, las aplicaciones y los datos. Las organizaciones están moviendo aplicaciones, como el correo electrónico, el monitoreo de la seguridad y la administración de la base de datos a la nube pública.

- Acceso no autorizado a los centros de datos, etc.
- Tiempo de inactividad del servidor durante los períodos de mantenimiento
- Vulnerabilidades de software del sistema operativo de la red
- Pérdida de datos
- Vulnerabilidad de desarrollo de aplicaciones web o de cliente/servidor.

## IMPORTANTE

### Dominios en Sistemas de Información

1. **Dominio de Usuario**  
   Incluye a cualquier persona con acceso al sistema de información de una organización: todos los empleados, clientes y partners contractuales.

2. **Dominio de Dispositivo**  
   Se refiere a cualquier computadora y otros dispositivos conectados a una red de computadoras.

3. **Dominio de Instalaciones Físicas**  
   Incluye todas las instalaciones utilizadas por una organización, así como las medidas de seguridad física empleadas para proteger dichas instalaciones.

4. **Dominio LAN**  
   Conjunto de dispositivos conectados localmente por cables o ondas de radio.

5. **Dominio de Nube Privada**  
   Incluye cualquier servidor privado, recursos e infraestructura de TI disponibles solo para miembros de una organización a través de Internet.

6. **Dominio de Nube Pública**  
   Incluye todos los servicios de computación alojados por un proveedor de nube o servicio de Internet que están disponibles para el público y compartidos entre organizaciones.

### Modelos de Servicio en la Nube

- **Software como Servicio (SaaS)**  
  Ofrece a las organizaciones software alojado de manera centralizada accesible por los usuarios a través de Internet.

- **Plataforma como Servicio (PaaS)**  
  Proporciona una plataforma que permite a una organización desarrollar, ejecutar y administrar sus aplicaciones en el hardware del servicio con herramientas provistas por el proveedor.

- **Infraestructura como Servicio (IaaS)**  
  Proporciona recursos de computación virtualizados, como hardware, software, servidores, almacenamiento y otros componentes de infraestructura a través de Internet.

## Rootkits y backdoors

### Backdoor

Un **backdoor** (puerta trasera) es un tipo de acceso no autorizado o oculto a un sistema informático, red o software. Los backdoors son creados intencionalmente o como resultado de una vulnerabilidad explotada por atacantes. Su propósito es permitir a los usuarios malintencionados eludir los mecanismos de seguridad convencionales, como la autenticación o la verificación de permisos.

Los backdoors pueden ser instalados de diversas formas:
- Mediante la explotación de vulnerabilidades en el sistema.
- A través de malware que instala el acceso sin que el usuario se dé cuenta.
- Creación intencionada por desarrolladores para facilitar el mantenimiento o el acceso futuro.

**Características de un backdoor:**
- Difícil de detectar.
- Permite acceso remoto al sistema.
- Puede servir como canal para realizar otras actividades maliciosas, como el robo de información o la ejecución de comandos.

### Rootkit

Un **rootkit** es un conjunto de herramientas de software que permite a un atacante obtener acceso privilegiado (root) a un sistema y mantenerse oculto durante el mayor tiempo posible. Los rootkits pueden modificar el funcionamiento del sistema operativo para ocultar su presencia y la de otros programas maliciosos.

**Tipos de rootkits:**
- **User-mode rootkits**: Operan en el nivel de usuario del sistema operativo, afectando aplicaciones o procesos sin alterar el núcleo del sistema.
- **Kernel-mode rootkits**: Funcionan a nivel del núcleo del sistema operativo, lo que los hace más peligrosos ya que pueden modificar funcionalidades básicas del sistema.
- **Bootkits**: Afectan el proceso de arranque del sistema, cargándose antes de que se inicie el sistema operativo y siendo extremadamente difíciles de eliminar.

**Características de un rootkit:**
- Oculta la presencia de malware.
- Puede deshabilitar herramientas de seguridad del sistema.
- A menudo se utiliza para mantener acceso persistente y sigiloso a un sistema comprometido.

Ambos, **backdoors** y **rootkits**, son usados por atacantes para comprometer la seguridad de un sistema y obtener control a largo plazo sin ser detectados.

# Ingeniería Social

La **ingeniería social** es una técnica utilizada por atacantes para manipular psicológicamente a las personas con el fin de obtener información confidencial, acceder a sistemas o cometer fraudes. A diferencia de los ataques técnicos, la ingeniería social se basa en el **comportamiento humano** y en explotar la confianza, la ignorancia o la falta de atención de las víctimas.

## Conceptos Clave de la Ingeniería Social

### 1. ¿Qué es la Ingeniería Social?
Es el arte de influenciar a las personas para que revelen información sensible o realicen acciones que comprometan la seguridad de sistemas y datos. Se aprovecha de la tendencia humana a confiar en otros, así como de la falta de conocimientos sobre amenazas cibernéticas.

### 2. Tácticas Comunes de Ingeniería Social

- **Phishing**  
  Envío de correos electrónicos fraudulentos que parecen provenir de una fuente confiable para engañar a las personas a revelar contraseñas o descargar malware.

- **Spear Phishing**  
  Un ataque dirigido hacia un individuo o grupo específico, con mensajes personalizados que aumentan la probabilidad de éxito.

- **Vishing (Voice Phishing)**  
  Uso de llamadas telefónicas para engañar a las víctimas y obtener información sensible como contraseñas o números de tarjeta de crédito.

- **Smishing (SMS Phishing)**  
  Similar al phishing, pero se realiza a través de mensajes SMS. El atacante envía mensajes con enlaces maliciosos o pide información confidencial.

- **Baiting**  
  Técnica en la que el atacante deja un dispositivo físico, como una memoria USB infectada con malware, en un lugar donde la víctima lo encuentre y lo conecte a su computadora.

- **Pretexting**  
  El atacante crea un pretexto o una historia falsa para engañar a la víctima, haciéndola creer que necesita dar acceso o información confidencial.

- **Quid pro quo**  
  Promete un beneficio a la víctima a cambio de información o acceso a un sistema. Por ejemplo, el atacante se hace pasar por un técnico de soporte que ofrece "ayuda" a cambio de credenciales.

- **Tailgating o Piggybacking**  
  El atacante sigue a una persona autorizada a través de una puerta de seguridad para acceder a áreas restringidas sin tener credenciales.

- **Shoulder Surfing**  
  Técnica de observación en la que el atacante se coloca físicamente cerca de la víctima para espiar mientras introduce sus contraseñas o datos sensibles.

- **Dumpster Diving**  
  Búsqueda de información sensible en la basura, como documentos, contraseñas o dispositivos desechados que aún pueden contener datos útiles.

### 3. Técnicas Psicológicas Utilizadas en Ingeniería Social

- **Autoridad**  
  Los atacantes se hacen pasar por figuras de autoridad, como un jefe, gerente o miembro del departamento de TI, para hacer que las víctimas confíen en ellos y revelen información.

- **Urgencia**  
  Crear una sensación de urgencia para presionar a la víctima a tomar decisiones apresuradas, como revelar información o hacer clic en un enlace antes de pensarlo bien.

- **Simpatía o Confianza**  
  Ganarse la simpatía o confianza de la víctima mediante la creación de una relación amigable o manipulando emociones.

- **Reciprocidad**  
  Los atacantes ofrecen algo a la víctima, creando una sensación de obligación que puede llevar a la víctima a corresponder con información o acceso.

### 4. Defensa Contra la Ingeniería Social

- **Educación y Concienciación**  
  Las personas deben estar capacitadas para reconocer las tácticas de ingeniería social y estar alerta ante solicitudes sospechosas de información.

- **Autenticación Multifactor (MFA)**  
  Utilizar más de un método de autenticación para proteger cuentas y sistemas, dificultando el acceso a los atacantes que solo tienen credenciales básicas.

- **Políticas de Seguridad**  
  Implementar políticas claras para el manejo de información sensible, acceso a sistemas y la verificación de solicitudes antes de actuar.

- **Detección de Ingeniería Social**  
  Enseñar a los usuarios a detectar señales de un posible ataque de ingeniería social, como urgencia excesiva, correos electrónicos no solicitados o solicitudes fuera de lo común.

- **Simulaciones de Ataques**  
  Realizar simulaciones de phishing y otros ataques de ingeniería social para entrenar al personal y mejorar su capacidad de respuesta.

# Resumen de Ataques Cibernéticos

## 1. Bombas Lógicas
Las bombas lógicas son programas maliciosos que se activan al cumplirse ciertas condiciones, como la fecha o la hora. Pueden eliminar datos, corromper archivos o realizar otras acciones perjudiciales en el sistema infectado.

## 2. Ransomware
El ransomware es un tipo de malware que cifra los archivos de la víctima y exige un rescate, generalmente en criptomonedas, para restaurar el acceso a los datos. Este ataque puede causar pérdidas significativas tanto financieras como de reputación.

## 3. DDOS (Denegación de Servicio Distribuida)
Los ataques DDoS buscan saturar un servidor, servicio o red con un tráfico excesivo, lo que impide que los usuarios legítimos accedan a ellos. Se utilizan redes de bots (botnets) para llevar a cabo estos ataques a gran escala.

## 4. DNS (Sistema de Nombres de Dominio)
Los ataques DNS pueden incluir la manipulación de registros DNS o el envenenamiento de caché DNS, permitiendo a los atacantes redirigir el tráfico a sitios maliciosos. Esto puede resultar en el robo de credenciales o la propagación de malware.

## 5. Ataques de Capa 2
Estos ataques ocurren en la capa de enlace de datos del modelo OSI e incluyen técnicas como la suplantación de dirección MAC y el sniffing de tráfico. Son difíciles de detectar y pueden comprometer la integridad de la red.

## 6. MITM (Hombre en el Medio)
Los ataques de Hombre en el Medio permiten a un atacante interceptar y modificar la comunicación entre dos partes sin que estas lo sepan. Esto puede llevar al robo de información confidencial, como credenciales y datos personales.

## 7. 0day
Las vulnerabilidades 0day son fallos de seguridad que son desconocidos para los desarrolladores de software y no tienen un parche disponible. Los atacantes pueden explotarlas para obtener acceso no autorizado a sistemas antes de que se pueda mitigar la vulnerabilidad.

## 8. Keyloggers
Los keyloggers son programas o dispositivos que registran las pulsaciones de teclas de un usuario. Pueden ser utilizados por atacantes para robar credenciales, información personal y realizar fraudes.


## Redes inálambricas

## 1. Grayware
Grayware se refiere a software que, aunque no es necesariamente malicioso, puede comprometer la privacidad y la seguridad del usuario. Incluye aplicaciones que muestran anuncios intrusivos, recopilan datos sin consentimiento o alteran el funcionamiento del dispositivo. Ejemplos comunes son adware y spyware.

## 2. SMiShing
SMiShing es una variante del phishing que utiliza mensajes de texto (SMS) para engañar a los usuarios y obtener información personal o financiera. Los atacantes envían mensajes fraudulentos que suelen contener enlaces a sitios web maliciosos o solicitan la descarga de aplicaciones dañinas.

## 3. Puntos de Acceso No Autorizados (Evil Twin)
Los puntos de acceso Evil Twin son redes Wi-Fi falsas que imitan redes legítimas. Los atacantes crean estas redes para atraer a usuarios desprevenidos, permitiendo la interceptación de datos personales y credenciales. Una vez conectados, los atacantes pueden monitorizar y manipular la comunicación del usuario.

## 4. Inhibidores de Radiofrecuencia
Los inhibidores de radiofrecuencia son dispositivos que bloquean las señales de comunicación inalámbrica. Se utilizan para interferir con la comunicación entre dispositivos, lo que puede impedir el acceso a redes Wi-Fi o la comunicación de datos entre dispositivos móviles. Su uso puede ser ilegal y se asocia con actividades maliciosas.

## 5. Bluejacking y Bluesnarfing
- **Bluejacking:** Es el envío no autorizado de mensajes a dispositivos Bluetooth cercanos. Aunque generalmente se considera una broma, puede ser utilizado para molestar o confundir a otros usuarios.
- **Bluesnarfing:** Es una técnica más maliciosa que permite a los atacantes acceder a la información de un dispositivo Bluetooth sin el conocimiento del propietario. Esto puede incluir contactos, mensajes y otros datos sensibles.

## 6. Ataques contra Protocolos de Wi-Fi
Los ataques contra protocolos de Wi-Fi incluyen diversas técnicas diseñadas para explotar vulnerabilidades en las redes inalámbricas. Ejemplos comunes son:
- **WPA/WPA2 Cracking:** Utiliza técnicas como ataques de diccionario para descifrar contraseñas de redes Wi-Fi.
- **Deauthenticating Attacks:** Desconectan a los usuarios de la red, permitiendo al atacante capturar información cuando el usuario intenta volver a conectarse.

# Ataques de Aplicaciones

## 1. Secuencias de Comandos entre Sitios (XSS)
Las secuencias de comandos entre sitios (XSS) son vulnerabilidades que permiten a un atacante inyectar scripts maliciosos en páginas web vistas por otros usuarios. Esto puede resultar en el robo de cookies, información sensible o el desvío de sesiones.

## 2. Inyección de Código
La inyección de código es una técnica en la que un atacante inserta código malicioso en un programa para alterar su comportamiento. Esto puede incluir la inyección de SQL, donde se manipulan consultas a bases de datos para acceder o modificar información no autorizada.

## 3. Desbordamiento del Búfer
El desbordamiento del búfer ocurre cuando un programa escribe más datos en un búfer de los que puede manejar, lo que puede corromper datos adyacentes y permitir la ejecución de código malicioso. Esto puede ser explotado para obtener acceso no autorizado o tomar control del sistema.

## 4. Ejecuciones Remotas de Código (RCE)
Las ejecuciones remotas de código permiten a un atacante ejecutar código en un sistema objetivo desde una ubicación remota. Esto puede resultar en la toma de control total del sistema afectado y se puede lograr a través de vulnerabilidades en aplicaciones o servicios.

## 5. Otros Ataques a Aplicaciones
Existen diversos ataques adicionales que pueden comprometer la seguridad de las aplicaciones, incluyendo:
- **Ataques de Inyección XML:** Manipulación de datos XML para acceder o alterar información.
- **Cross-Site Request Forgery (CSRF):** Engañar a un usuario para que ejecute acciones no deseadas en una aplicación en la que está autenticado.
- **Manipulación de Parámetros:** Alteración de los parámetros de entrada para acceder a recursos no autorizados.

## 6. Defensa Contra Ataques de Aplicaciones
Para protegerse contra ataques a aplicaciones, se pueden implementar varias estrategias, tales como:
- **Validación y Saneamiento de Entradas:** Asegurarse de que todas las entradas de los usuarios sean validadas y filtradas para evitar inyecciones.
- **Uso de Controles de Acceso:** Implementar políticas de acceso adecuadas para garantizar que solo los usuarios autorizados puedan acceder a ciertos recursos.
- **Parcheo Regular:** Mantener todas las aplicaciones y sistemas actualizados para cerrar vulnerabilidades conocidas.

## 7. Spam
El spam se refiere a la práctica de enviar mensajes no solicitados, a menudo de carácter comercial, a un gran número de usuarios. Esto puede saturar bandejas de entrada y ser utilizado para realizar fraudes o propagación de malware.

## 8. Suplantación de Identidad (Phishing)
La suplantación de identidad es una técnica en la que un atacante se hace pasar por una entidad confiable para engañar a los usuarios y obtener información sensible, como contraseñas o datos financieros. Puede realizarse a través de correos electrónicos, mensajes de texto o sitios web falsos.



## Conclusión

La ingeniería social es una amenaza seria que aprovecha el comportamiento humano para comprometer la seguridad. La mejor defensa es la educación y la concienciación, así como el uso de buenas prácticas de seguridad, como la autenticación multifactor y políticas estrictas para la gestión de la información.

