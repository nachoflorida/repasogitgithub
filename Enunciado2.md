# Pasos a seguir (2ª parte):
Recordad editar los ficheros que modifiquéis con Visual Studio Code

# Simular un conflicto

  Un conflicto aparece cuando en un mismo fichero existen versiones distintas en local y remoto.
  Vamos a simular uno y ver cómo lo podemos resolver:

**1. Entra en tu repositorio de GitHub con un navegador y edita el archivo `carta_bienvenida.md`**

- En la línea 4 añade: `* Añadimos esta línea para generar un conflicto`
- Guarda los cambios y haz commit desde el repositorio online.


**2. Ahora, en tu repositorio local, con el Visual Studio Code, edita el mismo fichero**

- Añade el texto: `Archivo modificado por: Nacho`

- Guarda (Ctrl + s)
- Haz commit 
- Sube los cambios al repositorio remoto

¡¡ El conflicto está servido !!
No nos deja subir los cambios, ya que hay contenidos diferentes en local y en remoto del fichero `carta_bienvenida.md`.
Nos recomienda que bajemos los archivos que tenemos en remoto. 

- Haremos un pull desde `origin` hasta `main`.

Visual Code Studio nos informa de la existencia del conflicto. Aparece una **C** sobre el fichero `carta_bienvenida.md`, en el apartado llamado 'Merge Changes'. O quizás aparece una **!** al lado del fichero `carta_bienvenida.md`.


**3. Editamos el fichero, y aparecen las dos versiones.**

Tendremos que seleccionar 'manualmente' cuál es la versión correcta, o integrar nosotros los cambios. 

En este caso, yo he optado por aceptar los dos cambios.

- Guarda (Ctrl + s)
- Haz commit 
- Sube los cambios al repositorio remoto

# Crear una rama nueva, modificar ficheros, y juntarlos a `main`

Vamos a crear una rama nueva para programar una nueva funcionalidad y que no afecte a todo lo que ya llevamos hecho en la rama `main`.

- La llamaremos `funcionalidad1` (Busca el comando para crear una rama nueva).
- Nos aseguramos que estamos en la nueva rama (Busca el comando para cambiar a otra rama).

**4. Editamos el fichero `carta_bienvenida.md` y le añadimos el texto:**  `Texto añadido desde la rama funcionalidad1`

- Guarda (Ctrl + s)
- Haz commit 

**5. Editamos el fichero `README.md` y le añadimos:**
`Texto añadido desde la rama funcionalidad1`
- Guarda (Ctrl + s)
- Haz commit

**6. Ahora lleva estos cambios a la rama main:**

- Haz un checkout a la rama `main`.
- Desde `main`, haz un merge con `funcionalidad1`. De este modo llevaremos los cambios hechos en `funcionalidad1` a la rama `main`.

**7. Sube los cambios que hay en `main` a GitHub**

**8. Comprueba en GitHub que se han subido correctamente los cambios.**
