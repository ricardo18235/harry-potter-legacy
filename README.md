# Harry Potter Legacy

# Documentación de la Aplicación de Personajes de Harry Potter

Esta aplicación **Vue.js** obtiene datos de la API de Harry Potter y muestra los personajes en una interfaz amigable para el usuario. La aplicación permite a los usuarios filtrar personajes basándose en su casa y linaje, y también proporciona una funcionalidad de búsqueda para encontrar personajes por nombre.

# Estructura de Datos
La aplicación mantiene los siguientes datos:

**message**: Un mensaje de saludo.  
**personajes**: Un array para almacenar los personajes obtenidos de la API.  
**personaje**: Un objeto para almacenar los detalles de un solo personaje.  
**personajesBkp**: Un array de respaldo para almacenar la lista original de personajes.  
**categoriasCasas**: Un array para almacenar las casas únicas en el universo de Harry Potter.  
**categoriasLinaje**: Un array para almacenar los linajes únicos en el universo de Harry Potter.  
**categoriasSeleccionadas**: Un array para almacenar los filtros de casa seleccionados.  
**linajeSeleccionado**: Un array para almacenar los filtros de linaje seleccionados.  
**buscador**: Una cadena para almacenar la consulta de búsqueda.  
**personajeAMostrar**: Un objeto para almacenar el personaje que se mostrará en el modal.  
**dataApiHarry**: Un array para almacenar los datos brutos obtenidos de la API.  
**favoritos**: Un array para almacenar los personajes favoritos del usuario.  
**urlImagen**: Una cadena para almacenar la URL de la imagen de marcador de posición.  

# Métodos
La aplicación incluye los siguientes métodos:

**dataHarry(url)**: Obtiene datos de la API de Harry Potter y los almacena en dataApiHarry. También llena categoriasCasas y categoriasLinaje con casas y linajes únicos, respectivamente.  
**mostrarModal(personaje)**: Muestra un modal con los detalles del personaje seleccionado.  
**agregarFavorito(personaje)**: Añade el personaje seleccionado a los favoritos del usuario y lo almacena en el almacenamiento local.  
**eliminarFavorito(personaje)**: Elimina el personaje seleccionado de los favoritos del usuario y actualiza el almacenamiento local.  

# Propiedades Computadas
La aplicación incluye las siguientes propiedades computadas:

**filtroCasas()**: Filtra los personajes basándose en los filtros de casa seleccionados y la consulta de búsqueda.  
**filtroLinaje()**: Filtra los personajes basándose en los filtros de linaje seleccionados y la consulta de búsqueda.  

# Almacenamiento Local
La aplicación utiliza el almacenamiento local para persistir los personajes favoritos del usuario a través de las sesiones.

# Punto de Montaje
La aplicación se monta en el elemento HTML con el id **app**.
