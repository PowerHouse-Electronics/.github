# PowerHouse Electronics

Este proyecto es parte de una asignatura universitaria y consiste en el desarrollo de una aplicación Android y una API para facilitar la venta de electrónicos.

## Descripción del proyecto

El objetivo principal de este proyecto es crear una plataforma que permita a los usuarios comprar electrónicos de manera fácil y segura. La aplicación Android proporcionará una interfaz intuitiva y amigable para que los usuarios puedan navegar por los productos, realizar compras y gestionar sus perfiles. La API se encargará de la lógica de negocio, la gestión de datos y la comunicación con la base de datos.

## Funcionalidades principales

### Usuarios
- Registro de usuarios: Los usuarios podrán crear cuentas en la aplicación proporcionando la información requerida.
- Inicio de sesión: Los usuarios podrán acceder a sus cuentas mediante un nombre de usuario y contraseña.
- Explorar productos: Los usuarios podrán ver una lista de productos disponibles para la venta, con información detallada sobre cada uno.
- Búsqueda y filtrado: Los usuarios podrán buscar productos específicos y aplicar filtros según categorías, precios.
- Carrito de compras: Los usuarios podrán agregar productos a un carrito de compras y realizar el proceso de compra.
- Perfiles de usuario: Los usuarios podrán gestionar su perfil, editar información personal, ver historial de compras.

### Administradores
- Administrar usuarios: Los administradores podrán ver y gestionar la lista de usuarios registrados, incluyendo la capacidad de editar sus perfiles y realizar acciones administrativas como la suspensión de cuentas.
- Administrar productos: Los administradores tendrán la capacidad de agregar, editar y eliminar productos del inventario. También podrán gestionar la información detallada de cada producto, como descripciones, precios y categorías.
- Gestión de pedidos: Los administradores podrán ver y administrar los pedidos realizados por los usuarios, incluyendo la capacidad de marcar pedidos como enviados o completados.
<!-- - Estadísticas y análisis: Los administradores tendrán acceso a estadísticas y análisis detallados sobre las ventas, ingresos y preferencias de los usuarios, lo que les permitirá tomar decisiones informadas sobre estrategias de venta y gestión de inventario.
Soporte al cliente: Los administradores podrán responder consultas y brindar soporte a los usuarios a través de un sistema de tickets o chat integrado en la aplicación. -->


## Tecnologías utilizadas

- Aplicación Android:
  - Lenguaje de programación: Java
  - Framework de desarrollo: Android SDK
  - Bibliotecas adicionales: Retrofit para la comunicación con la API, Picasso para la carga de imágenes.

- API:
  - Lenguaje de programación: Javascript
  - Framework: NodeJS
  - Base de datos: MongoDB

## Estructura del repositorio

El repositorio está organizado de la siguiente manera:

- `/app-android`: Contiene el código fuente de la aplicación Android.
- `/api`: Contiene el código fuente de la API.
<!-- - `/documentación`: Contiene documentación adicional relacionada con el proyecto. -->

## Instalación y configuración

Sigue los siguientes pasos para instalar y configurar el proyecto:

1. Clona este repositorio en tu máquina local.
2. Asegúrate de tener [Node.js v16.16.0 LTS](https://nodejs.org) instalado en tu sistema.
3. Asegúrate de tener [MongoDB](https://www.mongodb.com) instalado y en funcionamiento en tu sistema.
4. Ejecuta `npm install` para instalar todas las dependencias del proyecto.
5. Ejecuta `npm run start` para iniciar la aplicación.

### Configuración de MongoDB

1. Abre el archivo `connection.js` en la carpeta `connection`.
2. Asegúrate de que la URL de conexión de MongoDB esté configurada correctamente, asegurándote de que coincida con tu configuración local de MongoDB.

```javascript
const connectDB = async() => {
    try {
        // Configura la URL de conexión de MongoDB
        await mongoose.connect("mongodb://127.0.0.1:27017/FinalProject",);
        console.log('DB online');
    }
```
## Contribución

Este proyecto es parte de un trabajo universitario y no se aceptarán contribuciones externas en este momento.

## Equipo de desarrollo

- Fernando de la Cruz - Desarrollador Android
- Alejandro Orbe - Desarrollador Backend
- Ulises Velazquez - Documentador

## Licencia

Este proyecto se distribuye bajo la licencia MIT. Puedes consultar el archivo [LICENSE](LICENSE) para obtener más información.
