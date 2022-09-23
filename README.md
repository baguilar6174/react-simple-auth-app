# React Simple Auth App

Una vez que el proyecto se haya clonado accedemos al direcotorio de la aplicación y ejecutamos el comando `yarn` o `npm i` para obtener todas las dependencias. En mi caso

```bash
cd simple-auth-app/
yarn
```

En este punto puede probar la correcta ejecución de tu aplicación, si estas usando yarn, con el siguiente comando:

```bash
yarn run dev
```

## Dependencias utilizadas

* _axios_: Librería utilizada para hacer solicitudes HTTP
* _eslint-plugin-react-hooks_: Nos ayuda a controlar errores y nos brinda ayuda cuando tengamos algún error de codificación de nuestros hooks.
* _redux_: Gestor de estados de la aplicación.
* _sass_: Permite usar SASS en lugar de simple CSS (si instalas esta extensión asegúrate de cambiar las extensiones de tus ficheros css a scss, además reemplaza la extensión importaciones en los ficheros `App.tsx` y `main.tsx`)
* _bootstrap_: Framework de CSS
* _react-hook-form_: Librería para el manejo y validación de formularios
* _react-router-dom_: Gestor de rutas para React

## Estructura de directorios

En mis proyectos suelo utilizar la siguiente estructura de directorios:

```
├── src/
    ├── assets/
    │   ├── images/
    │   ├── icons/
    │   ├── fonts/
    │   ├── ...
    ├── components/
    │   └── Component1.component.tsx
    ├── data/
    ├── hooks/
    ├── layout/
    ├── models/
    ├── pages/
    │   └── page1/
    │       ├── components/
    │       └── Page1.page.tsx
    ├── redux/
    │   ├── ...
    │   ├── store.tsx
    ├── routes/
    │   ├── routes.tsx
    ├── services/
    ├── utilities/
		...
    ├── App.scss
    ├── App.tsx
    ├── favicon.ico
    ├── index.scss
    └── main.tsx
...
```

1. El directorio `assets` contiene todos los recursos multimedia como imágenes, fuentes, íconos, incluso aquí se pueden agregar archivos para la internacionalización de la aplicación en un directorio `i18n`.
2. El directorio `components` contiene todos los componentes globales de tu aplicación por ejemplo: alertas personalziadas, laoders o componentes de paginación.
3. El directorio `data` contiene constantes que puedes usar en tu aplicación, aquí puedes incluir rutas, o enumeraciones.
4. El directorio `hooks` contiene hooks personalizados que ayudarán a abstraer lógica de tu aplicación.
5. El directorio `layout` contiene los elementos principales por los que se conforma tu aplicación, por lo general suelen ser cuatro: Header, Sidebar, Footer y Skeleton.
6. El directorio `models` contiene los modelos que usarás en tu aplicación ya que estamos usando Typescript, es importante mantener un correcto tipado en toda la aplicación.
7. El directorio `pages` contiene las páginas por las que esta conformada tu aplicación, yo acostumbro a crear un direcotrio por cada conjunto de páginas (por ejemplo el directorio `users` contendrá las páginas: `UsersList.page.tsx`, `UsersCreate.page.tsx` y `UserDetails.page.tsx`) además puedes crear un subdirectorio componentes en caso de que todas estas páginas compartan componentes.
8. El directorio `redux` contiene la configuración del estado global de neustra aplicaicón, esto lo veremos más adelante.
9. El directorio `routes` contiene un archivo con la definición de las rutas de tu aplicación.
10. El directorio `services` contiene la definición de axios para las peticiones HTTP, aquí puedes crear interceptores que te ayuden a agregar cabeceras o manejar los errores de mejor manera.
11. Finalmente, el directorio `utilities` lo puedes usar para alamcenar funciones globales en tu aplicación por ejemplo: una función de conversión de divisas, un formateador de fechas, etc.

## Author

- Website - [www.bryan-aguilar.com](https://www.bryan-aguilar.com/)
- Medium - [baguilar6174](https://baguilar6174.medium.com/)
- LinkeIn - [baguilar6174](https://www.linkedin.com/in/baguilar6174)
- Email - [bryan.aguilar6174@gmail.com](mailto:bryan.aguilar6174@gmail.com)

## Estado del proyecto

Actualmente este proyecto contiene un simple login (fake) usando el localstorage, se puede hacer uso de alguna api de autenticación.
