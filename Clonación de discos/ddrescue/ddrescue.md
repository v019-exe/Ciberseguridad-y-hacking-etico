# DDRESCUE

ddrescue es una herramieta que se usa para la recuperación de datos de discos duros o particiones dañadas.

## Características

1. Copia de datos en bloques: copia los datos de origen a un destino en bloques.
2. Registro de un archivo de mapa (logfile): Guarda un archivo de registro que lleva un seguimiento de las áreas copiadas con éxito, los sectores defectuosos y los bloques que deben volver a intentarse.
3. Reintento inteligente: Una vez qeu se ha copiado la mayor cantidad de datos posible, puede volver a intentar leer los bloques defectuosos multiples vecescon el fin de recuperar la máxima info posible.
4. Modo inverso: Si el disco está en mal estado, el programa también tiene un modo de funcionamiento inverso que comienza la lectura desde el final de larchivo hasta el principio, en vez de hacerlo secuencialmente, para eitar que se estropeen los sectores sanos.

## Sintaxis

```bash
ddrescue [opciones] origen destino logfile
```

## Opciones comunes
+ `-f`: obliga a sobreescribir el archivo de destino si ya existe.
+ `-n`: Hace la primera pasada sin intentar rescatar los sectores defectuosos.
+ `-r <n>`: Define cuantas veces se tiene que intentar recuerar los bloques defectuosos.
+ `-d`: Usa acceso directo al disco envez del sistema de archivos.

