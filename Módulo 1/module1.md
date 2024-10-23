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

## Conclusión

La ingeniería social es una amenaza seria que aprovecha el comportamiento humano para comprometer la seguridad. La mejor defensa es la educación y la concienciación, así como el uso de buenas prácticas de seguridad, como la autenticación multifactor y políticas estrictas para la gestión de la información.

