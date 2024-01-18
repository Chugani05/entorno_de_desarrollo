# Aplicación de transporte

## Actores
|  Actor | Usuario |
|---|---|
| Descripción  | Persona que utiliza el sistema de biblioteca para buscar, prestar y devolver libros.  |
| Características  | - Capacidad para buscar libros por título, autor, etc. - Capacidad para realizar préstamos y devoluciones. - Puede acceder a su historial de préstamos. |
| Relaciones | Interactúa con el caso de uso "Buscar Libro", "Prestar Libro", "Devolver Libro". |
| Referencias | Buscar Libro, Prestar Libro, Devolver Libro |
| Notas | - Los usuarios pueden tener diferentes niveles de acceso según su tipo (estudiante, profesor, etc.). |
| Autor | Rashi Chugani Narwanni |
| Fecha | 18/01/2024 |

|  Actor | Bibliotecario |
|---|---|
| Descripción  | Personal encargado de la gestión y administración del sistema de biblioteca.  |
| Características  | - Capacidad para gestionar el inventario de libros. - Puede registrar nuevos libros en el sistema. - Gestiona los préstamos y devoluciones. |
| Relaciones | Interactúa con el caso de uso "Gestionar Inventario", "Registrar Libro", "Gestionar Préstamos". |
| Referencias | Gestionar Inventario, Registrar Libro, Gestionar Préstamos |
| Notas | - Puede tener acceso a informes y estadísticas sobre el uso de la biblioteca. |
| Autor | Rashi Chugani Narwanni |
| Fecha | 18/01/2024 |

## Casos de uso
|  Caso de Uso	CU | Buscar Libro  |
|---|---|
| Fuentes  | Catálogo de la biblioteca  |
| Actor  | Usuario  |
| Descripción | Permite al usuario buscar libros en el catálogo de la biblioteca.  |
| Flujo básico | 1. El usuario inicia sesión en el sistema. 2. Navega al catálogo de libros. 3. Ingresa criterios de búsqueda (título, autor, etc.). 4. Examina los resultados de búsqueda. |
| Pre-condiciones | El usuario ha iniciado sesión en el sistema. |
| Post-condiciones  | El usuario visualiza una lista de libros que coinciden con los criterios de búsqueda.  |
| Requerimientos | Conexión a Internet para acceder al catálogo en línea.  |
| Notas | - Se pueden proporcionar filtros avanzados para mejorar la precisión de la búsqueda. |
| Autor | Rashi Chugani Narwanni |
| Fecha | 18/01/2024 |

|  Caso de Uso	CU | Prestar Libro  |
|---|---|
| Fuentes  | Catálogo de la biblioteca, Sistema de préstamos  |
| Actor  | Usuario  |
| Descripción | Permite al usuario solicitar el préstamo de un libro.  |
| Flujo básico | 1. El usuario busca el libro deseado. 2. Selecciona el libro y solicita el préstamo. 3. El sistema verifica la disponibilidad del libro. 4. Si está disponible, se registra el préstamo. |
| Pre-condiciones | El usuario ha iniciado sesión y ha encontrado un libro disponible. |
| Post-condiciones  | El libro es prestado al usuario y se actualiza su historial de préstamos.  |
| Requerimientos | El usuario no debe tener préstamos pendientes.  |
| Notas | - Se establece un período de préstamo y se generan recordatorios de vencimiento. |
| Autor | Rashi Chugani Narwanni |
| Fecha | 18/01/2024 |

|  Caso de Uso	CU | Gestionar Inventario  |
|---|---|
| Fuentes  | Catálogo de la biblioteca, Sistema de inventario  |
| Actor  | Bibliotecario  |
| Descripción | Permite al bibliotecario agregar, eliminar o actualizar libros en el inventario.  |
| Flujo básico | 1. El bibliotecario inicia sesión en el sistema. 2. Accede a la sección de gestión de inventario. 3. Agrega, actualiza o elimina información de libros. |
| Pre-condiciones | El bibliotecario ha iniciado sesión y tiene los permisos adecuados. |
| Post-condiciones  | El inventario se actualiza según las modificaciones realizadas por el bibliotecario.  |
| Requerimientos | Conexión a la base de datos del sistema de biblioteca.  |
| Notas | - Se pueden registrar detalles como la ubicación física de los libros en la biblioteca. |
| Autor | Rashi Chugani Narwanni |
| Fecha | 18/01/2024 |

|  Caso de Uso	CU | Gestionar Préstamos  |
|---|---|
| Fuentes  | Sistema de préstamos  |
| Actor  | Bibliotecario  |
| Descripción | Permite al bibliotecario gestionar los préstamos de libros realizados por los usuarios.  |
| Flujo básico | 1. El bibliotecario inicia sesión en el sistema. 2. Accede a la sección de gestión de préstamos. 3. Visualiza los préstamos activos y su estado. 4. Registra la devolución de libros. |
| Pre-condiciones | El bibliotecario ha iniciado sesión y tiene los permisos adecuados. |
| Post-condiciones  | El sistema registra la devolución de libros y actualiza el estado de los préstamos.  |
| Requerimientos | Conexión a la base de datos del sistema de biblioteca.  |
| Notas | - Se pueden generar multas por devoluciones tardías. |
| Autor | Rashi Chugani Narwanni |
| Fecha | 18/01/2024 |