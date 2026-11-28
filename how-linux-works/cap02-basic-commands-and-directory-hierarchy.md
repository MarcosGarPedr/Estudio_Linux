# Capítulo 2: Basic Commands and Directory Hierarchy


## Resumen
Este capítulo enseña los comandos principales de Linux y ofrece una visión general de como se estructura el sistema de directorios.

---

## 1. La shell
- **¿Qué es la shell?**
 La shell es el programa que interpreta todos los comandos que utilizamos para dar instrucciones a la máquina.
- **¿Qué es Bash y qué relación tiene con la Bourne shell (`sh`)?**
 Bash funciona como el transmisor entre nosotros y la shell. Es el encargado de llevar los comandos que nosotros introducimos a la shell para que ésta los interprete.
- **Entrada y salida estándar (stdin / stdout):** ¿qué son?
 Son los archivos o canales de entrada y salida por defecto. Nuestros inputs al pc entran por el canal stdin que por defecto es el teclado y el output sale por el canal stdout que por defecto es la pantalla.

---

## 2. Comandos básicos

| Comando | Para qué sirve | Ejemplo que he probado |
|---------|----------------|------------------------|
| `ls`    |                |                        |
| `cp`    |                |                        |
| `mv`    |                |                        |
| `touch` |                |                        |
| `rm`    |                |                        |
| `echo`  |                |                        |
| `cat`   |                |                        |

---

## 3. Navegar por directorios

| Comando | Para qué sirve | Ejemplo que he probado |
|---------|----------------|------------------------|
| `pwd`   |                |                        |
| `cd`    |                |                        |
| `mkdir` |                |                        |
| `rmdir` |                |                        |

- **Ruta absoluta vs ruta relativa:**
- **Qué significan `.`, `..` y `~`:**
- **Comodines (globbing):** `*` y `?`

```bash
# Un ejemplo de comodín que haya probado

```

---

## 4. Comandos intermedios

| Comando | Para qué sirve | Ejemplo que he probado |
|---------|----------------|------------------------|
| `grep`  |                |                        |
| `less`  |                |                        |
| `diff`  |                |                        |
| `file`  |                |                        |
| `find`  |                |                        |
| `head`  |                |                        |
| `tail`  |                |                        |
| `sort`  |                |                        |

---

## 5. Contraseña, shell y ficheros ocultos
- **Cambiar la contraseña (`passwd`):**
- **Dotfiles (ficheros que empiezan por `.`):** ¿qué son y cómo se ven?

---

## 6. Variables y `PATH`
- **Variable de shell vs variable de entorno:**
- **¿Qué es `PATH` y para qué sirve?**

```bash
echo $PATH
# Lo que me sale:

```

---

## 7. Caracteres especiales y edición en la línea de comandos
- **Caracteres especiales importantes:**
- **Atajos de teclado útiles** (Ctrl+A, Ctrl+E, Ctrl+U, Tab…):

---

## 8. Editores de texto
- **El editor que uso y por qué:**

---

## 9. Pedir ayuda

| Comando  | Para qué sirve |
|----------|----------------|
| `man`    |                |
| `--help` |                |
| `info`   |                |

---

## 10. Redirecciones y tuberías

| Símbolo | Qué hace | Ejemplo que he probado |
|---------|----------|------------------------|
| `>`     |          |                        |
| `>>`    |          |                        |
| `<`     |          |                        |
| `\|`    |          |                        |
| `2>`    |          |                        |

- **¿Qué es stderr y en qué se diferencia de stdout?**

---

## 11. Mensajes de error
- **Errores que me he encontrado y qué significaban:**
  - `No such file or directory` →
  - `Permission denied` →

---

## 12. Procesos

| Comando | Para qué sirve | Ejemplo que he probado |
|---------|----------------|------------------------|
| `ps`    |                |                        |
| `kill`  |                |                        |
| `jobs`  |                |                        |
| `fg` / `bg` |            |                        |

- **Ejecutar algo en segundo plano (`&`):**
- **Ctrl+C vs Ctrl+Z:**

---

## 13. Permisos de ficheros
- **Cómo leer los permisos de `ls -l`:**

```text
-rw-r--r-- 1 marcos marcos 64 nov 26 08:27 README.md
```

  - Tipo de fichero:
  - Permisos del propietario:
  - Permisos del grupo:
  - Permisos del resto:

- **`chmod` en modo número (ej. `644`, `755`):**
- **`chmod` en modo letras (ej. `u+x`):**
- **Enlaces simbólicos (`ln -s`):**

---

## 14. Archivar y comprimir

| Comando | Para qué sirve | Ejemplo que he probado |
|---------|----------------|------------------------|
| `gzip` / `gunzip` |      |                        |
| `tar`   |                |                        |

- **Diferencia entre archivar y comprimir:**
- **Opciones de `tar` que he usado:**

---

## 15. Jerarquía de directorios de Linux

| Directorio | Qué contiene |
|------------|--------------|
| `/bin`     |              |
| `/sbin`    |              |
| `/etc`     |              |
| `/home`    |              |
| `/root`    |              |
| `/tmp`     |              |
| `/var`     |              |
| `/usr`     |              |
| `/dev`     |              |
| `/proc`    |              |
| `/boot`    |              |
| `/lib`     |              |

---

## 16. Ejecutar comandos como superusuario
- **`sudo` vs `su`:**
- **¿Por qué no conviene trabajar siempre como root?**

---

## Problemas y cómo los resolví
-

## Lo que no tengo claro todavía
-

## Palabras clave
- **Shell:**
- **Glob / comodín:**
- **Variable de entorno:**
- **PATH:**
- **stdin / stdout / stderr:**
- **Tubería (pipe):**
- **PID:**
- **Permisos (modo):**
- **Enlace simbólico:**
