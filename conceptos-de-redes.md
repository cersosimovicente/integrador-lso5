# Ejercicios sobre Redes en Linux

## **Ejercicio 1: Configuración básica de una interfaz de red**
Configura una interfaz de red `eth0` con los siguientes parámetros:
- Dirección IP estática: `192.168.1.10`
- Máscara de red: `255.255.255.0`
- Puerta de enlace predeterminada: `192.168.1.1`

Realiza la configuración mediante el archivo `/etc/network/interfaces`.

---

## **Ejercicio 2: Verificación de configuración de red**
Verifica la configuración actual de todas las interfaces de red disponibles en el sistema. 

**Indicaciones:**
Utiliza un comando que muestre las direcciones IP, el estado de las interfaces y otros detalles relevantes.

---

## **Ejercicio 3: Añadir y eliminar una dirección IP secundaria**
1. Añade la dirección IP secundaria `10.0.0.10/24` a la interfaz `eth0`.
2. Comprueba que la IP ha sido añadida correctamente.
3. Elimina la dirección IP secundaria añadida en el paso anterior.

---

## **Ejercicio 4: Configuración de una ruta estática**
Configura una ruta estática en el sistema para alcanzar la red `172.16.0.0/24` utilizando el gateway `192.168.1.254`.

**Requerimientos:**
- Implementa esta configuración temporalmente mediante comandos.
- Documenta cómo hacerla persistente en el archivo `/etc/network/interfaces`.

---

## **Ejercicio 5: Prueba de conectividad**
Comprueba si la configuración TCP/IP está funcionando correctamente utilizando la dirección de loopback (`127.0.0.1`).

**Requerimientos:**
- Realiza un ping a `localhost`.
- Verifica que los paquetes enviados sean recibidos correctamente.

---

## **Ejercicio 6: Resolución de nombres utilizando `/etc/hosts`**
Configura la resolución de nombres en el archivo `/etc/hosts` para que la dirección IP `192.168.1.20` sea accesible con el nombre `servidor.local`.

**Indicaciones:**
- Realiza la modificación en el archivo `/etc/hosts`.
- Verifica que el nombre resuelva correctamente utilizando un comando de prueba.

---

