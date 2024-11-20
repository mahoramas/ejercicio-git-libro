# ejercicio-git-libro


# Paso inicial

## Clonar el repositorio
```code
bae2@jpexposito-VirtualBox:~$ git clone https://github.com/mahoramas/ejercicio-git-libro
Clonando en 'ejercicio-git-libro'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Recibiendo objetos: 100% (3/3), listo.
```

## Ejercicio 1

```code
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ git log
mkdir capitulos
cat > capitulos/capitulo1.txt
commit 76e06452518b3e1ea05d57319ceaf851bff95d2d (HEAD -> main, origin/main, origin/HEAD)
Author: Marcos Hernández Oramas <oramashernandez.educa@gmail.com>
Date:   Mon Nov 18 19:23:32 2024 +0000

    Initial commit

```
## Ejercicio 2
```code
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ cat > capitulos/capitulo2.txt
 El flujo de trabajo básico con Git consiste en:
 1- Hacer cambios en el repositorio.
 2- Añadir los cambios a la zona de intercambio temporal.
 3- Hacer un commit de los cambios.
```
``` code
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ git diff HEAD~2..HEAD
diff --git a/README.md b/README.md
index 9a06b52..e690d60 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,36 @@
-# ejercicio-git-libro
\ No newline at end of file
+# ejercicio-git-libro
+
+
+# Paso inicial
+
+## Clonar el repositorio
+```code
+bae2@jpexposito-VirtualBox:~$ git clone https://github.com/mahoramas/ejercicio-git-libro
+Clonando en 'ejercicio-git-libro'...
+remote: Enumerating objects: 3, done.
+remote: Counting objects: 100% (3/3), done.
+remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
+Recibiendo objetos: 100% (3/3), listo.
+```
+
:
```
## Ejercicio 3

```code
    git status
En la rama main
Tu rama está adelantada a 'origin/main' por 4 commits.
  (usa "git push" para publicar tus commits locales)
Cambios no rastreados para el commit:
  (usa "git add <archivo>..." para actualizar lo que será confirmado)
  (usa "git restore <archivo>..." para descartar los cambios en el directorio de trabajo)
        modificados:     README.md
Archivos sin seguimiento:
  (usa "git add <archivo>..." para incluirlo a lo que será confirmado)
        capitulos/Capitulo3.txt
sin cambios agregados al commit (usa "git add" y/o "git commit -a")ç
    git add .
    git commit -m "Añadido capitulo 3 y cambios al README"
[main af2c8e6] Añadido capitulo 3 y cambios al README
 2 files changed, 84 insertions(+)
 create mode 100644 capitulos/Capitulo3.txt
```
