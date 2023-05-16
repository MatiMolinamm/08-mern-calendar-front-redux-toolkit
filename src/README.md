//----------------------------------------------------------------------------//

1- react-big-calendar //npm i react-big-calendar
2- npm i date-fns
3- eventPropGetter => atributo de <Calendar/>, permite modificar estilos sobre lo seleccionado.
4- npm  i react-modal // paquete para generar modal. (ventana q se cierra y abre).
5- npm i react-datepicker // paquete para q aparezca modal de mini almanaque para seleccionar fechas.
6- npm i redux toolkit // npm i react-redux
7- generamos la carpeta store: 
*Configuramos el archivo store.js.
*Creamos los slices.
8-En el punto mas alto de la aplicacion <Provider store={ store }></>
9- creamos custom hooks para manejar el store de una forma centralizada.
10-useSelector from react redux. me permite obtener el estado.
11- middleware: (getDefaultMiddleware) => getDefaultMiddleware({
        serializableCheck: false
    }) // para que no tire error en las fechas. JS toma las fechas como string y debemos usar numero.

/---------------------------------------------------------------------------------------------------/
    CONEXION CON EL BACKEND
12-variables de entorno => import.meta.env //vienen configuradas en vite y cra de ptra forma
13- .env genero el archivo en la raiz del proyecto. las constantes van capitalizada con snakecase
*/ las variables de entorno no llegan al cliente. a menos q antepongamos VITE_ cuando estamos en vite ver para cra.
14- npm i axios
15- creo la carpeta api con los endpoint.
16- creo el hoock useAuthStore en lugar de thunks.
17-establece en el localStorage el token que viene del back dentro del useAuthStorage

18-sweet alert => modal predefinido
19- interceptores en axios. lo usa para evalidar el token. en api calendarApi
20- en el AppRouter uso el checkAuthToken, retornado por el useAuthStore.







