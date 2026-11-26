# Capítulo 1: The Big Picture

**Fecha:** 2026-11-26

## Resumen en una frase
Este capítulo ofrece una visión simplificada de como funciona Linux, que elementos lo componen y como interactúa con los distintos componentes del sistema
para hacer posible que este funcione. 

## Ideas clave
- **Los niveles de abstracción de un sistema Linux: hardware, kernel y espacio de usuario.**
  - El hardware es el sistema físico en sí mismo (CPU, RAM, tarjetas de red etc.)
  - El Kernel es el software encargado de gestionar el hardware y las distintas tareas, además es la interfaz principal entre el hardware y los programas.
  - El espacio de usuario es el constituido por el conjunto de programas que estan corriendo en el sistema.
- **Las tareas del kernel: procesos, memoria, drivers y llamadas al sistema.**
  - Procesos: Gestiona los procesos dando tiempo y turnos de CPU así como gestionando el acceso a recursos del sistema.
  - Memoria: Gestiona la memoria otorgada a cada proceso y el acceso a datos y memoria que los propios procesos necesitan.Se asegura de que un proceso no 
   pueda leer ni escribir la memoria de otro (ni la del kernel). Para eso usa la memoria virtual y la MMU.
  - Drivers: El software que el Kernel utiliza para hacer de interfaz entre el hardware y los procesos.
  - Llamadas al sistema: Es el mecaniSmo que los procesos de usuario utilizan para pedir al kernel determinadas acciones que ellos no pueden hacer.
- **Modo kernel vs modo usuario: ¿qué diferencia hay y por qué existe?**
  El kernel se ejecuta en modo kernel, con acceso total a la CPU y la memoria. Los procesos se ejecutan en modo usuario, con acceso restringido, para que 
  un fallo en un programa no tumbe todo el sistema.
- **Usuarios y root: ¿qué tiene de especial root?**
  Un usuario de Linux es aquel que puede correr sus propios procesos y archivos en el sistema. Un sistema Linux puede tener distintos usuarios, con sus procesos
  y archivos separados. Cada usuario maneja sus procesos y archivos con ciertos límites pero no los de los otros usuarios.
  El usuario root es el administrador del sistema, puede administrar procesos y archivos de otros usuarios. También es un usuario normal a ojos del kernel 
  y sus procesos corren en modo usuario, no en modo kernel. Tiene más permisos (puede tocar procesos y ficheros de cualquier usuario), pero sigue pidiendo cosas 
  al kernel mediante llamadas al sistema igual que los demás.
  El kernel identifica a los usuarios por un número (UID), no por su nombre.

## Palabras clave
- **Kernel** 
- **Proceso**
- **Estado de un proceso**
- **Llamadas al sistema**
- **Context switch**
- **Time slice**
- **Memory ManagEment Unit (MMU)**
- **Memoria virtual**
