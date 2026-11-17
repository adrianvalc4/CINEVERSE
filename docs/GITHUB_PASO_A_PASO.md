# Publicar CINEVERSE en GitHub

## A. Crear el repositorio en GitHub

1. Inicia sesión en GitHub.
2. Pulsa `+` y elige `New repository`.
3. Escribe `CINEVERSE` como nombre.
4. Añade una descripción: `Proyecto académico de sitio web de películas`.
5. Selecciona `Public` o `Private` según indique el ingeniero.
6. No marques `Add a README`, `.gitignore` ni licencia porque estos archivos ya existen en el proyecto local.
7. Pulsa `Create repository`.
8. Copia la dirección HTTPS que GitHub muestra, con esta forma: `https://github.com/TU-USUARIO/CINEVERSE.git`.

## B. Preparar el repositorio local

El paquete `CINEVERSE_repo_local_listo.zip` ya incluye un repositorio Git inicializado y un primer commit. Después de descomprimirlo, abre la carpeta `CINEVERSE_primera_entrega` en Visual Studio Code y abre `Terminal > New Terminal`.

Primero registra tu identidad de GitHub (reemplaza los valores por los tuyos):

```bash
git config user.name "Tu nombre"
git config user.email "tu-correo-de-GitHub"
git commit --amend --reset-author --no-edit
```

Esto actualiza el autor del primer commit para que GitHub lo asocie a tu cuenta si el correo coincide con uno verificado en GitHub.

## C. Conectar y publicar en GitHub

Copia la dirección HTTPS de tu repositorio. En la terminal ejecuta, una línea a la vez:

```bash
git remote add origin https://github.com/TU-USUARIO/CINEVERSE.git
git push -u origin main
```

Reemplaza `TU-USUARIO` por tu usuario de GitHub. Si Git pide autenticarte, completa el inicio de sesión en el navegador.

## D. Comprobar la subida

1. Vuelve a la página del repositorio en GitHub.
2. Actualiza la página.
3. Debes ver `index.html`, las demás páginas, la carpeta `css`, `README.md` y `docs`.
4. Abre `index.html` desde GitHub para comprobar que el archivo fue subido.

## E. Actualizar después de realizar cambios

Cada vez que modifiques el proyecto y quieras guardar una nueva versión:

```bash
git add .
git commit -m "Descripción breve del cambio"
git push
```

`git add` prepara los cambios, `git commit` guarda una versión local y `git push` la sube al repositorio remoto.
