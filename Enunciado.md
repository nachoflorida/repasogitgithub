# Pasos a seguir

**1. Abrimos una consola de comandos (en Windows ejecutamos la aplicación "Símbolo del sistema" o la orden "cmd").**

**2. En nuestro disco local, vamos a la carpeta donde tenemos nuestros desarrollos. En mi caso:**
   ```
    cd C:\Users\Nacho\21-React\
   ```

**3. Descargamos el que tenemos en el repositorio remoto (en GitHub) creado por el profesor, es decir, vamos a *clonar* ese repositorio:**
   ```
   git clone URL_DEL_REPOSITORIO
   ```
Ya tenemos una copia del repositorio remoto en la máquina local. 
**¡¡ NO CERRAMOS LA CONSOLA DE ÓRDENES !!**
A partir de ahora trabajaremos en local y subiremos los cambios en el repositorio remoto.

**4. Modificamos, en local, el archivo README.md para añadirle tu nombre con una cabecera (Header) de nivel 1.**

**5. Subiremos los cambios a GitHub de este modo:**

- Guarda el archivo README.md modificado (Ctrl + s).
- Añade los cambios en el Stage Area.
- Haz un commit con el comentario "añado mi nombre".
- Después haz un push.
- Refresca la página del navegador donde tenemos el repositorio remoto en GitHub, para comprobar los cambios.

**6. Añadiremos al archivo README.md una lista con 3 cosas que nos gustaría conseguir al finalizar el ciclo/curso**

**7. Subiremos los cambios a GitHub de este modo:**

- Guarda el archivo README.md modificado (Ctrl + s)
- Añade los cambios en el Stage Area.
- Haz un commit con el comentario "añado lista cosas fin ciclo/curso".
- Después haz un push.
- Refresca la página del navegador donde tenemos el repositorio remoto en GitHub, para comprobar los cambios.

**8. Descargaremos de internet el logo de GitHub y lo guardaremos en nuestro repositorio local.**
    
- Añadiremos esa imagen al stage Area, para subirla a nuestro repositorio remoto.
- Añade el archivo de la imagen del logo en el Stage Area.
- Haz un commit con el comentario "añado el logo de GitHub".
- Después haz un push.
- Refresca la página del navegador donde tenemos el repositorio remoto en GitHub, para comprobar los cambios.

**9. Modificaremos el archivo README.md para que nos muestre el logo de GitHub.**
- Guarda el archivo README.md modificado (Ctrl + s)
- Añade los cambios en el Stage Area.
- Haz un commit con el comentario "añado logo GitHub".
- Después haz un push.
- Refresca la página del navegador donde tenemos el repositorio remoto en GitHub, para comprobar los cambios.

**10. Añadiremos el texto: `Ya hemos practicado con GitHub`, en el fichero README.md**
- Seguiremos las acciones habituales

**11. Deshaciendo el último cambio subido a GitHub.**
Imagínate que modificas un archivo o varios para implementar una mejora, has guardado los cambios y los has subido a GitHub, pero pruebas la app y ahora falla más que antes. Por tanto, decides dejarlo todo como estaba antes de los últimos cambios realizados.

Es decir, *vamos a deshacer la última acción realizada*:

- Desde la consola de comandos revisamos los últimos 10 commits que hemos hecho: 
    ```
    git log -10
    ```

 - Tomaremos el identificador del commit que queremos restaurar.
    ```
    git reset --hard <identificador_del_commit>`
    ```
 - Enviaremos los cambios a la rama master del repositorio remoto (GitHub):
    ```
    git push origin HEAD:master --force
    ```
