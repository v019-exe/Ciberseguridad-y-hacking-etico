# Clonación de discos usando dd, data duplicator

DD es una herramienta muy poderosa en linux para copiar datos de bajo nivel entre dispositivos, archivos o particiones. Se utiliza principalmente para clonar discos o particiones, crear imágenes ISO, backups entre otros. Trabaja diretamente con el contenido binario, copiando bloque por bloque sin interpretar el contenido. Es versátil pero peligroso si se usa de manera incorrecta, ya que puede sobrescribir datos sin avisar.

```bash
dd if=<origen> of=<destino> [opciones]
```

+ `if=<origen>`: Origen del disco a copiar.
+ `of=<destino>`: Destino del disco a copiar.

## Ejemplo básico
```bash
dd if=/dev/sda of=/dev/sdb bs=64K conv=noerror,sync
```

Esto copia el disco /dev/sda a /dev/sdb, usando bloques de 64K.

## Parámetros clave de DD
1. `if=` (input file):
    + Es el origen de los datos a copiar.

2. `of=` (Output file):
    + El destino donde se escribirán los datos copiados

3. `bs=` (block size):
    + Especifica el tamaño de los bloques que se leerán y escribirán.

4. `count` (copiar 100 bloques de 1M por ejemplo):
    + Especifica cuátnos bloques se leerán/escribirán. Si no se especifica, `dd` continuará hasta que todo el archivo o dispositivo de origen se copie.
    + Solo si quieres copiar una parte del archivo o disco, puedes definir cuantos bloques se deben copiar.

```bash
dd if=/dev/sda of=/dev/sdb bs=64K count=100
```
Esto copiará los 100 primeros bloques del disco /dev/sda a /dev/sdb de 64K.

5. `skip=` (skip n bytes):
    + Salta una cantidad específica de bloques al leer del archivo de origen.
    + Util si no quieres copiar todo el archivo o disco desde el inicio.

6. `seek=` (seek n bytes):
    + Salta una cantidad específica de bloques al escribir en el archivo de destino.
    + Util para escribir datos en una ubicación específica del archivo de destino.

```bash
seek=10
```
Escribir a partir del bloque 10 en el destino.

7. `conv=` (conversion):
+ Modifica como se copian los datos, opciones comunes:
    + `noerror`: Continua copiando incluso si encuentra errores de lectura.
    + `sync`: Alinea los bloques, rellenando con ceros en caso de errores de lectura.
    + `notrunc`: No trunca el archivo de salida (deja los datos que ya existian antes).

```bash
conv=noerror,sync
```

