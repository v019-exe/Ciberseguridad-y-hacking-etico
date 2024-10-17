# RSYNC
rsync es una herramienta de sincronización y transferencia de archivos en sistemas Unix y linux.

## Características
1. Sincronización diferencial: Solo copia las diferencias entre origen y destino.
2. Transferencia remoa: Puede sincronizar archivos entre un sistema local y uno remoto a través de SSH.
3. Preservación de atributos: Mantiene los atributos de los archivos como permisos, propietario, grupo, fechas de modificación, etc.
4. Renaudación de transferencias: Si una transferencia se interrumpe, rsync es capaz de renaudarla desde donde se paró.
5. Compresión: Puede comprimir los datos durante la transferencia para ahorrar ancho de banda.
6. Exclusiones: Permite excluir ciertos archivos o directorios de la sincronización.

## Sintaxis
```bash
rsync [opciones] origen destino
```

## Opciones comunes
+ `-a`: Modo archivo (sincroniza de manera recursiva y preserva permisos, tiempos de modificación, etc.)
+ `-v`: Verbose (muestra información detallada sobre la transferencia)
+ `-z`: Comprime los datos durante la transferencia
+ `-h`: formato humano (muestra información de manera más legible)
+ `--delete`: Elimina los archivos en el destino qe no existen en el origen.
+ `--dry-run`: Simula la transferencia sin hacer cambios reales, muy util para ver que pasaria.

