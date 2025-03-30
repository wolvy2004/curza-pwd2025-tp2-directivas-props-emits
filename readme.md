# Trabajo practico N°2 📹

En este trabajo practico veremos lo aprendido en las ultimas clases 

- directivas: ``v-for`` `` v-show``
- props
- emits

## Manos a la obra 🔨
Vamos a crear una aplicación vue con el comando ``npm run vite`` recuerden si en proyect_name escriben . les crea la instalacion en la raiz de la carpeta (opcional)
una vez creada limpiaremos el archivo app para dejarlo listo para poder trabajar.

#### Creación del componente ``Card`` 🪪
- Creamos un componente al cual llamaremos ``CardComponent.vue``  tendra como  ``prop`` **movie** que sera de tipo `` Pelicula ``
el cual deberá mostrar los datos de la misma
- Este componente tendra ademas un ``emit`` **update_likes** que devolverá la cantidad de likes modificados, solo se podra hacer por usuario un solo like si presiona nuevamente lo quitara.
- Puede existir una pelicula que no tenga una portada para mostrar, en este caso de acuerdo a si existe o no podremos mostrar un mensaje **Portada no disponible**.
 
### Interface Pelicula 📽️
Como vimos en clase vamos a crear una interface llama ``Pelicula`` la cual tendra los siguientes atributos

| Atributo     | Tipo  | Requerido |
|:-------------|:----- |:---------:|
|**id**        |number | S         |
|**titulo**    |String | S         |
|**anio**      |Number | S         |
|**genero**    |String | S         |
|**director**  |String | S         |
|**portada**   |String | N         |
|**likes**     |Number | S         |

Para tener organizado nuestros archivos crearemos una carpeta ``interfaces`` en la cual agregaremos el archivo ``Pelicula.ts``

En la raiz del la carpeta clonada tienen una carpeta ``resources`` (ahora bien escrito) la cual tiene un archivo con las peliculas de ejemplo para que puedan trabajar, las cuales pueden importar a la ``app.vue`` para trabajar.

Es este componente el cual se va a encargar de renderizar la lista de peliculas en formato **Cards** para lo cual tendremos que usar la directiva para este proposito.


> Como en el trabajo anterior podremos **estilizar** nuestras ``Cards`` de forma personalizada, los invito a que liberen su creatividad para crear diseños unicos!!! 🦾