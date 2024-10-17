# PARTCLONER
Es una herramienta de software diseñada para clonar particiones de disco y sistemas de archivos en linux y otros sistemas Unix.

## Características

1. Copia eficiente: Partclone copia solo los bloques utilizados en un sistema de archivos.
2. Compatibilidad con varios sistemas de archivos: Soporta diferentes tipos de sistemas de archivos, como ext2, ext3, ext4, reiserfs, xfs, jfs, btrfs, etc.
3. Restauración: No solo permite clonar, también permite restaurar los datos a partir de una imagen de copia de seguridad.
4. Generación de imágenes comprimidas: Partclone puede crear imágenes comprimidas de las particiones, lo que ahorra espacio en disco.

## Sintaxis

```bash
partclone.<filesystem> [opciones]
```

## Opciones comunes
+ `-s`: Especifica el origen
+ `-o`: Especifica la salida
+ `-r`: Usa esta opción para restaurar
+ `-j`: Permite usar la compresión al crear la imagen
+ `-q`: Habilita el modo silencioso.

