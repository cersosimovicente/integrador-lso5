# Ejercicios de Administración de Usuarios y Permisos en GNU/Linux

## **Ejercicio 1: Crear usuarios y asignarles un grupo primario**
Crea tres usuarios llamados `user1`, `user2` y `user3`. Asigna a cada uno un grupo primario específico:
- `user1` al grupo `ventas`
- `user2` al grupo `compras`
- `user3` al grupo `administracion`

---

## **Ejercicio 2: Cambiar permisos de directorios**
Crea tres directorios: `dir1`, `dir2`, y `dir3`. Cambia los permisos de manera que:
- `user1` tenga acceso completo a `dir1`.
- `user2` tenga solo permisos de lectura en `dir2`.
- `user3` tenga acceso completo a `dir3` y permita acceso de solo lectura a su grupo.

---

## **Ejercicio 3: Verificar pertenencia a grupos**
Agrega a `user1` al grupo secundario `administracion` y a `user2` al grupo secundario `ventas`. Verifica los grupos a los que pertenece cada usuario.

---

## **Ejercicio 4: Crear un esquema de permisos colaborativo**
Implementa un sistema en el que:
- El grupo `ventas` tenga acceso a `dir1`.
- El grupo `compras` tenga acceso a `dir2`.
- El grupo `administracion` tenga acceso a `dir3`.
- Los usuarios que no pertenezcan a los grupos no puedan acceder a esos directorios.

---

## **Ejercicio 5: Configuración avanzada de permisos**
Cambia los permisos de `dir3` para que:
- El propietario tenga permisos completos.
- El grupo tenga permisos de lectura y escritura.
- Otros usuarios no tengan ningún permiso.

## Material Entregable:
Documento en formato PDF o Markdown donde expliquen:
Qué hicieron en cada paso.
El propósito de cada comando utilizado.
