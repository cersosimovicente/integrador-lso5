# Ejercicios de Administración de Procesos en Linux

## Ejercicio 1: Identificar procesos en el sistema
**Objetivo:** Usar el comando `ps` para listar procesos y comprender su salida.

1. Ejecute el comando `ps aux`.
2. Responda las siguientes preguntas:
   - ¿Cuál es el PID del proceso `bash` que está en ejecución?
   - ¿Qué usuario inició este proceso?
   - ¿Cuál es el porcentaje de CPU y memoria que utiliza?

---

## Ejercicio 2: Terminar un proceso
**Objetivo:** Usar el comando `kill` para finalizar un proceso específico.

1. Abra el editor `nano` desde la terminal.
2. Utilizando otra terminal:
   - Identifique el PID del proceso `nano`.
   - Finalice el proceso utilizando el comando `kill`.

---

## Ejercicio 3: Cambiar la prioridad de un proceso
**Objetivo:** Usar `renice` para modificar la prioridad de un proceso en ejecución.

1. Ejecute el comando `yes` en una terminal.
2. Cambie su prioridad a 10 mientras está en ejecución utilizando el comando `renice`.

---

## Ejercicio 4: Uso de tuberías
**Objetivo:** Practicar la redirección de salidas con tuberías.

1. Liste todos los procesos en ejecución que contienen la palabra `systemd`.
2. Utilice comandos en tuberías para contar cuántos procesos relacionados con `systemd` están en ejecución.

---

## Ejercicio 5: Ejecutar un proceso en segundo plano
**Objetivo:** Ejecutar un proceso con `nohup` y comprobar que continúa tras cerrar la sesión.

1. Ejecute el comando `sleep` durante 300 segundos en segundo plano utilizando `nohup`.
2. Verifique que el proceso continúa ejecutándose después de cerrar la sesión.
