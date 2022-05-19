# sesion7-tarea-grupo
3. ¿Qué tengo que hacer?
En esta práctica tienes que instalar y configurar XAMPP, una plataforma de desarrollo de aplicaciones
web que incorpora el servidor web Apache, el sistema gestor de bases de datos MySQL y los lenguajes de
programación PHP y Perl9. A partir de ahora, usaremos XAMPP para desarrollar y probar la aplicación
web que estás desarrollando.
Por otro lado, tienes que dividir la estructura de las páginas de tu sitio web en múltiples
ficheros y tienes que utilizar PHP para combinarlos en uno solo. Detecta la partes que sean
comunes a diferentes páginas de tu sitio web (por ejemplo, la cabecera con el título, la barra de navegación
y el pie de página) y ponlas en ficheros independientes. De este modo te puedes crear una plantilla a
partir de la cual se genera cualquier página web de tu sitio web.
Además, tienes que programar con PHP las páginas web que reciban los datos enviados a partir
de los formularios que has realizado en las prácticas anteriores. Por ahora, estas páginas simplemente
tienen que mostrar los datos recibidos (ya no datos ficticios) para comprobar que todo funciona
correctamente. En próximas prácticas almacenarás estos datos en una base de datos.
En concreto, tienes que modificar o crear las páginas que se indican con un color de relleno oscuro en
la Figura 1.
Página control de acceso No es una página visible. Controla el acceso a la parte privada para los
usuarios registrados. Por ahora, se debe limitar el acceso a cuatro posibles usuarios cuyos datos
(nombre de usuario, contraseña) están almacenados directamente en esta página (en una próxima
práctica se accederá a una base de datos para consultar los usuarios permitidos). Si el usuario está
registrado, mediante una redirección en la parte del servidor se debe mostrar la página con el menú
de usuario registrado; si el usuario no está registrado, mediante una redirección en la parte del
servidor se debe mostrar la página principal del sitio web con un mensaje de error que explique al
usuario lo que ha pasado.
Página “Crear álbum” Contiene un formulario con los datos necesarios para crear un álbum (título y
descripción).
Respuesta “Solicitar álbum” Muestra una confirmación de que se ha registrado la solicitud de un
álbum y también muestra el coste del álbum calculado a partir de la solicitud del usuario. Se debe
emplear la tabla de tarifas que aparece en la Práctica 3. Como todavía no existen álbumes y fotos
en una base de datos, debes emplear unos valores ficticios para el número de páginas y número
de fotos del álbum; sin embargo, sí que debes tener en cuenta el resto de parámetros que elija el
usuario en el formulario de solicitud.
Respuesta “Página con el formulario de registro como nuevo usuario” Muestra los datos que
el usuario ha introducido en el formulario de registro. Se debe comprobar que se ha escrito al-
go en el nombre de usuario, en la contraseña y en repetir contraseña, y que contraseña y repetir
contraseña coinciden. La validación del resto de campos del formulario se implementará en una
próxima práctica. Importante: en esta página no se debe mostrar la fotografía de perfil seleccionada
por el usuario, la subida de ficheros al servidor se implementará en una próxima práctica.
Página con el listado resultado de una búsqueda Además del ejemplo de resultado de una bús-
queda que ya contiene (datos estáticos), muestra los datos reales que el usuario ha introducido en
el formulario de búsqueda.
Página detalle foto Muestra el detalle de la foto seleccionada (foto, título, fecha, país, álbum de fotos
y usuario al que pertenece). A esta página se puede llegar desde cualquier otra página en la que
aparezcan fotos de la aplicación, como por ejemplo, la página principal (las últimas fotos subidas)
o la página con el listado resultado de una búsqueda. Por ahora, se deben mostrar los datos de
dos fotos distintas que están almacenados directamente en esta página (en una próxima práctica
se accederá a una base de datos para obtener los datos reales); la elección de la foto a mostrar
dependerá de si el identificador de la foto que se reciba es un número par o impar.
