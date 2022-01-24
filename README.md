# vuebots

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out the [documentation](https://nuxtjs.org).

## Special Directories

You can create the following extra directories, some of which have special behaviors. Only `pages` is required; you can delete them if you don't want to use their functionality.

### `assets`

The assets directory contains your uncompiled assets such as Stylus or Sass files, images, or fonts.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/assets).

### `components`

The components directory contains your Vue.js components. Components make up the different parts of your page and can be reused and imported into your pages, layouts and even other components.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/components).

### `layouts`

Layouts are a great help when you want to change the look and feel of your Nuxt app, whether you want to include a sidebar or have distinct layouts for mobile and desktop.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/layouts).


### `pages`

This directory contains your application views and routes. Nuxt will read all the `*.vue` files inside this directory and setup Vue Router automatically.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/get-started/routing).

### `plugins`

The plugins directory contains JavaScript plugins that you want to run before instantiating the root Vue.js Application. This is the place to add Vue plugins and to inject functions or constants. Every time you need to use `Vue.use()`, you should create a file in `plugins/` and add its path to plugins in `nuxt.config.js`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/plugins).

### `static`

This directory contains your static files. Each file inside this directory is mapped to `/`.

Example: `/static/robots.txt` is mapped as `/robots.txt`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/static).

### `store`

This directory contains your Vuex store files. Creating a file in this directory automatically activates Vuex.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/store).


# vuebots | OBJETIVO 

Desarrollar una interfaz con VueJs que permita correr una carrera de bots visible sobre un mapa de Google Maps.

La competencia consiste en que el usuario indica un punto sobre el mapa al que todos los bots deben acercarse en línea recta cambiando su posición cada 1 segundo. Los bots se encuentran ubicados de manera aleatoria en la ciudad donde vives.

Debes cumplir con cada uno de los siguientes puntos:

La interfaz debe mostrar un mapa de Google Maps y un recuadro donde se listan los bots. El número inicial de bots que empiezan en la competencia debe ser un número aleatorio entre 5 y 10.

1. Los bots se mueven en dirección al punto marcado por el usuario como meta. Cada bot solo puede hacer un movimiento cada 1 segundo de una distancia aleatoria entre 50 y 100 metros.


2. Cada bot tiene una batería que dura 100 unidades, y cada cambio de posición gasta un número aleatorio entre 10 y 30 unidades.


3. Cuando un bot quede sin batería debe detenerse por 6 segundos para volver a empezar con 100 unidades.


4. Se debe mostrar un botón “Agregar nuevo Bot”, que al presionarse incrementa en 1 el número de bots en competencia. Al agregarse, se ubica de manera aleatoria en la ciudad y de inmediato inicia su trayecto a la meta


5. La interfaz debe mostrar de manera fácil el estado de toda la competencia, estado de los bots, posición de cada uno, distancia hacia la meta y todo lo que considere útil para el usuario


6. El bot que esté más cerca a la meta debe mostrarse con color verde. El último con color rojo, y el resto con color amarillo.


7. Alojar la prueba en algún servicio de tal manera que nos puedas enviar la url para nosotros visualizarlo en funcionamiento.
