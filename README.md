# sumativa-2
links de imagenes para probar:

https://i.ibb.co/mCtzYmyG/bad-born-blood.jpg / 
https://i.ibb.co/QjvHW79G/descarga.jpg /
https://i.ibb.co/Xfb4MTKV/mago-pastor.webp

prompt usado:

Crea una aplicación web mobile-first de una sola página (HTML, CSS y JS puros, sin frameworks) llamada ManhwaTracker. Es un catálogo personal de manhwas con las siguientes características:
Diseño:
Tema oscuro moderno. Colores: fondo #0d0d0d, cards #1a1a1a, acento rojo #e63946, acento rojo oscuro #7a0000, texto #f0f0f0, texto secundario #888888. Tipografía moderna (Google Fonts). Diseño mobile-first, responsive.
Formulario (bottom sheet modal al presionar FAB "+" flotante):
Campos: Título (texto, obligatorio), Género (select: Romance, Acción, Fantasía, Terror, Drama), Capítulo actual (número, mínimo 0), Estado (select: Leyendo, Pendiente, Completado), URL de portada (texto, opcional). Validación con expresiones regulares y sanitización de inputs. Sin uso de innerHTML con datos del usuario, usar textContent o createElement.
Catálogo:
Cards verticales a ancho completo. Cada card muestra: portada (o placeholder si no hay URL), título, género, capítulo, estado. Dentro de cada card: input numérico para actualizar el capítulo directamente, selector para cambiar el estado directamente, botón eliminar.
Filtros y búsqueda:
Tabs fijos en la parte superior: Todos / Leyendo / Pendiente / Completado. Buscador por título que se expande con ícono. Ambos filtran el DOM en tiempo real.
Contadores dinámicos:
Mostrar cantidad de manhwas por estado debajo de los tabs.
Persistencia:
Todo se guarda y carga desde localStorage. Al cargar la página renderizar los datos guardados.
Estructura del código:
Funciones modulares y reutilizables con nombres semánticos: renderList(), addItem(), deleteItem(), updateItem(), filterByStatus(), searchByTitle(), saveToStorage(), loadFromStorage(), sanitizeInput(), validateForm(). Sin código monolítico. Comentarios en el código indicando qué partes fueron asistidas por IA.
Seguridad:
Evitar XSS: no usar innerHTML con datos del usuario. Sanitizar todos los inputs. Escapar datos dinámicos.
Entregar todo en un único archivo index.html con CSS y JS embebidos.
