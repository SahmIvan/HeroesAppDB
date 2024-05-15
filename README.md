# Superhero App

La Superhero App es una aplicación Android que permite a los usuarios explorar una lista de superhéroes y obtener detalles sobre cada uno de ellos. A continuación, se proporciona una descripción detallada de la aplicación, incluyendo las funcionalidades básicas, la arquitectura utilizada, las bibliotecas integradas y los pasos para ejecutar la aplicación.

## Funcionalidades Básicas

1. **Lista de Superhéroes**: La aplicación muestra una lista de superhéroes disponibles, con su nombre y posición.

2. **Detalle del Superhéroe**: Al hacer clic en un superhéroe de la lista, se muestra una pantalla de detalle con información más detallada, incluyendo el nombre, la posición y una imagen del superhéroe.

## Arquitectura

La arquitectura de la Superhero App está basada en el patrón de arquitectura de **Modelo-Vista-ViewModel (MVVM)**, que proporciona una separación clara de las responsabilidades y facilita la escalabilidad y mantenimiento del código. La estructura de archivos del proyecto se organiza de la siguiente manera:

- **data**: Contiene las clases relacionadas con el manejo de datos, como entidades, DAOs, repositorios y la base de datos Room.

- **di**: Incluye los módulos Dagger Hilt para la inyección de dependencias en la aplicación.

- **presentation**: Aquí se encuentran las clases de la interfaz de usuario, incluyendo activities, adapters y viewmodels.

### Componentes Principales:

- **Entidades (Entities)**: Representan los objetos de datos que se almacenan en la base de datos. En este caso, las entidades son los superhéroes.

- **DAOs (Data Access Objects)**: Proporcionan métodos para acceder a la base de datos y realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar) en las entidades.

- **Repositorios (Repositories)**: Actúan como una capa de abstracción entre los DAOs y los viewmodels, proporcionando métodos para obtener y manipular datos.

- **ViewModels**: Contienen la lógica de presentación de la aplicación y se encargan de mantener y gestionar el estado de la interfaz de usuario. Se comunican con los repositorios para obtener los datos necesarios y los exponen a las vistas a través de observables.

## Bibliotecas Utilizadas

La Superhero App utiliza las siguientes bibliotecas principales:

- **Room**: Para la persistencia de datos en la base de datos SQLite de la aplicación.

- **Dagger Hilt**: Para la inyección de dependencias, facilitando la gestión de componentes y la modularidad del código.

- **Picasso**: Para cargar y mostrar imágenes de superhéroes en la interfaz de usuario de manera eficiente.

## Pasos para Ejecutar la Aplicación

Para ejecutar la Superhero App en un dispositivo o emulador Android, sigue estos pasos:

1. Clona el repositorio de GitHub de la aplicación en tu máquina local.
2. Abre el proyecto en Android Studio.
3. Asegúrate de tener configurado un dispositivo Android o un emulador en tu máquina.
4. Haz clic en el botón "Run" (Ejecutar) en Android Studio para compilar y ejecutar la aplicación en tu dispositivo o emulador.
5. Una vez que la aplicación se haya instalado y ejecutado con éxito, podrás explorar la lista de superhéroes y ver los detalles de cada uno de ellos.

Con estos pasos, podrás disfrutar de la Superhero App y explorar el emocionante mundo de los superhéroes en tu dispositivo Android.
