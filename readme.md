# Trabajo práctico N°2 📹

En este trabajo práctico veremos lo aprendido en las últimas clases:

- Directivas: ``v-for`` `` v-show``
- Props
- Emits

## Manos a la obra 🔨

Vamos a crear una aplicación Vue con el comando ``npm run vite``. Recuerden que si en `project_name` escriben un punto (`.`), se creará la instalación en la raíz de la carpeta (opcional). Una vez creada, limpiaremos el archivo `App.vue` para dejarlo listo para poder trabajar.

#### Creación del componente ``Card`` 🪪

- Creamos un componente al cual llamaremos ``CardComponent.vue``. Tendrá como ``prop`` **movie**, que será de tipo ``Pelicula``, el cual deberá mostrar los datos de la misma.
- Este componente tendrá además un ``emit`` **update_likes** que devolverá la cantidad de likes modificados. Solo se podrá hacer un solo like por usuario; si presiona nuevamente, lo quitará.
- Puede existir una película que no tenga una portada para mostrar. En este caso, de acuerdo a si existe o no, podremos mostrar un mensaje: **Portada no disponible**.

### Interfaz Pelicula 📽️

Como vimos en clase, vamos a crear una interfaz llamada ``Pelicula``, la cual tendrá los siguientes atributos:

| Atributo     | Tipo   | Requerido |
|:-------------|:------ |:---------:|
| **id**       | number | S         |
| **titulo**   | String | S         |
| **anio**     | Number | S         |
| **genero**   | String | S         |
| **director** | String | S         |
| **portada**  | String | N         |
| **likes**    | Number | S         |

Para tener organizados nuestros archivos, crearemos una carpeta ``interfaces`` en la cual agregaremos el archivo ``Pelicula.ts``.

En la raíz de la carpeta clonada, tienen una carpeta ``resources`` (ahora bien escrita), la cual contiene un archivo con las películas de ejemplo para que puedan trabajar. Estas pueden ser importadas a ``App.vue`` para trabajar.

Es este componente el que se va a encargar de renderizar la lista de películas en formato **Cards**, para lo cual tendremos que usar la directiva correspondiente.

> Como en el trabajo anterior, podremos **estilizar** nuestras ``Cards`` de forma personalizada. ¡Los invito a liberar su creatividad para crear diseños únicos! 🦾