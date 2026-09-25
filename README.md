# entregaGit-GitHub
En esta práctica voy a demostrar que sé trabajar con un repositorio Git local y un repositorio remoto en GitHub.

## Problemas y dudas

1- Después de haber creado el archivo-4.txt no me he acordado de salir de la carpeta-4 a la principal. Por eso al hacer git status no me salían todas las carpetas reflejadas. Al realizar add solo se ha hecho archivo-4.txt, dejando sin hacer la modificación de README.md y el resto de archivos y carpetas. Me he dado cuenta al hacer de nuevo status.

2- Me ha vuelto a suceder no estar en la carpeta correcta. Al hacer git pull se me había guardado la imágen en carpeta contactos. Me he dado cuenta, y he vuelto a hacerlo desde la carpeta principal.

## Historial de la práctica

1-Historial después del primer commit.

$ git log --oneline
436ede6 (HEAD -> main) Crear estructura inicial del proyecto
77cbbd3 (origin/main, origin/HEAD) Initial commit

2-Historial de feature/contacto.

git log --oneline
5cdf121 (HEAD -> feature/contacto) Añadir página de contacto
436ede6 (origin/main, origin/HEAD, main) Crear estructura inicial del proyecto
77cbbd3 Initial commit

3- Historial después del merge.

$ git merge feature/contacto
Updating 436ede6..5cdf121
Fast-forward
 contacto/contacto.html | 96 ++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 96 insertions(+)
 create mode 100644 contacto/contacto.html

 4- Historial después de actualizar desde GitHub.

 $ git log --oneline
1d947f1 (HEAD -> main, origin/main, origin/HEAD) Añadir Imagen desde GitHub
5cdf121 (origin/feature/contacto, feature/contacto) Añadir página de contacto
436ede6 Crear estructura inicial del proyecto
77cbbd3 Initial commit

5- Historial de feature/contacto después de incorporar la rama principal.

$ git merge main
Updating 5cdf121..1d947f1
Fast-forward
 GitHub-1.jpg | Bin 0 -> 49542 bytes
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 GitHub-1.jpg