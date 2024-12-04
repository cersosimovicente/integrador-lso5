# Laboratorio: Gestión de Particiones en Linux

## Introducción
En este laboratorio, aprenderás a gestionar particiones en Linux utilizando herramientas como `fdisk`, `parted` y el sistema de archivos ext4. Este laboratorio incluye pasos para crear, formatear y montar particiones, además de verificar su funcionamiento.

## Objetivos
1. Comprender cómo listar discos y particiones disponibles.
2. Crear y formatear particiones.
3. Montar particiones y configurarlas para el montaje automático al inicio del sistema.
4. Explorar el uso de herramientas comunes para la gestión de particiones.

## Requisitos previos
- Sistema operativo Linux (Ubuntu recomendado).
- Privilegios de superusuario (`sudo`).
- Un disco adicional (físico o virtual) para trabajar.

---

## Actividades

### 1. Listar discos y particiones
1. Abre una terminal y utiliza el comando `lsblk` para listar los discos y particiones disponibles:

2. Verifica el estado de los discos disponibles utilizando el comando `fdisk`:

3. Identifica el disco donde crearás una nueva partición (por ejemplo, `/dev/sdb`).

**Tarea:** Documenta cuál es el disco seleccionado.

---

### 2. Crear una nueva partición
1. Abre el gestor de particiones `fdisk` para el disco seleccionado:

2. Sigue estos pasos dentro de `fdisk`:
   - Presiona `n` para crear una nueva partición.
   - Selecciona `p` para crear una partición primaria.
   - Especifica el número de partición (por ejemplo, `1`).
   - Acepta los valores predeterminados para el primer y último sector o define el tamaño deseado (por ejemplo, `+1G` para 1 GB).
   - Presiona `w` para escribir los cambios y salir.

3. Verifica los cambios con:


**Tarea:** Describe los pasos seguidos y los resultados observados.

---

### 3. Formatear la partición
1. Formatea la nueva partición con el sistema de archivos ext4:

2. Verifica el sistema de archivos:


**Tarea:** Documenta los comandos ejecutados y sus resultados.

---

### 4. Montar la partición
1. Crea un directorio donde montar la partición (por ejemplo, `/mnt/lab`):

2. Monta la partición en el directorio creado:

3. Verifica que la partición está montada:


**Tarea:** Copia un archivo al directorio montado y verifica que se almacena correctamente.

---

### 5. Configurar el montaje automático
1. Abre el archivo `fstab` para edición:

2. Agrega la siguiente línea al final del archivo:
   ```
   /dev/sdb1   /mnt/lab   ext4   defaults   0   2
   ```
3. Guarda los cambios y verifica el montaje:
   ```bash
   sudo mount -a
   ```

**Tarea:** Reinicia el sistema y confirma que la partición se monta automáticamente.

---

## Evaluación
Responde las siguientes preguntas:
1. ¿Cuál es el propósito del archivo `fstab`?
2. ¿Qué herramientas puedes utilizar además de `fdisk` para gestionar particiones?
3. Explica los pasos necesarios para desmontar una partición de forma segura.

---

## Limpieza (opcional)
1. Desmonta la partición:

2. Opcional: Elimina la partición creada si ya no la necesitas:
   ```bash
   sudo fdisk /dev/sdb
   ```
   Sigue los pasos dentro de `fdisk`:
   - Presiona `d` para eliminar la partición.
   - Presiona `w` para guardar los cambios.

---

## Conclusión
Has completado un laboratorio sobre gestión de particiones en Linux. Este conocimiento es fundamental para administrar almacenamiento en servidores y estaciones de trabajo.

**Tarea final:** Entrega un informe que incluya capturas de pantalla de cada paso realizado y las respuestas a las preguntas de evaluación.
