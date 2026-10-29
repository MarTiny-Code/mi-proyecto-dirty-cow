Dirty COW (CVE-2016-5195) — Estudio de Escalada de Privilegios en Linux

Proyecto de laboratorio en el que estudio y ejecuto el exploit Dirty COW (CVE-2016-5195), una de las vulnerabilidades más famosas del kernel de Linux, en un entorno controlado. El objetivo: entender de primera mano cómo un fallo del kernel permite a un usuario sin privilegios escalar hasta root (administrador).

Qué es Dirty COW

Dirty COW (Dirty Copy-On-Write) fue una vulnerabilidad del kernel de Linux descubierta en 2016. Explota una condición de carrera en el mecanismo Copy-On-Write de gestión de memoria, permitiendo a un usuario normal escribir en archivos de solo lectura y, a partir de ahí, escalar privilegios a root. Afectó a prácticamente todas las distribuciones Linux de la época, lo que la hizo especialmente grave.

Qué hice en este laboratorio
Estudié el funcionamiento del exploit y la vulnerabilidad subyacente.
Utilicé la herramienta Dirty COW sobre el laboratorio proporcionado en el curso para explotar la vulnerabilidad.
Logré la escalada de privilegios a root, confirmada con la flag del ejercicio.
Analicé por qué funciona el ataque y cómo se mitiga (actualización del kernel).
Qué demuestra
Comprensión de vulnerabilidades a nivel de kernel y de la escalada de privilegios en Linux.
Capacidad de analizar y ejecutar un exploit real en un entorno seguro.
Conciencia de la importancia del parcheo como medida defensiva (la mitigación de Dirty COW fue actualizar el kernel).
Contenido
dirty.cpp — código de la herramienta/exploit utilizada en el laboratorio.
Tecnologías y conceptos

Linux · Kernel · C++ · Escalada de privilegios · CVE-2016-5195 · Análisis de exploits

🚩 4GEEKS{Y0u_G0t_R00t} — flag del ejercicio (escalada a root conseguida).

Proyecto académico con fines educativos, ejecutado en un entorno de laboratorio aislado sobre un sistema preparado para ello.
