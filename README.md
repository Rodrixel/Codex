Simulador de Cubo de Rubik 3D
Descripción General
Este proyecto es un simulador de Cubo de Rubik 3D desarrollado con HTML, CSS y JavaScript, utilizando la biblioteca Three.js. Permite a los usuarios interactuar con un cubo de Rubik virtual en 3D, realizar movimientos estándar del cubo (U, D, L, R, F, B y sus inversos), mezclar el cubo, reiniciarlo y resolverlo siguiendo un tutorial paso a paso basado en el método para principiantes. El simulador cuenta con animaciones suaves, colores nativos del cubo de Rubik y un diseño responsivo para una experiencia de usuario atractiva.
Características

Cubo 3D Interactivo: Visualiza un cubo de Rubik en 3D con colores realistas (blanco, amarillo, rojo, naranja, verde, azul).
Rotaciones de Caras: Realiza movimientos estándar del cubo (U, U', D, D', L, L', R, R', F, F', B, B') mediante botones.
Controles de Órbita: Rota todo el cubo arrastrando con el ratón para verlo desde cualquier ángulo.
Mezclar y Resolver: Mezcla el cubo con movimientos aleatorios y resuélvelo revirtiendo la secuencia de mezcla.
Tutorial para Principiantes: Guía paso a paso con notación estándar para resolver el cubo.
Diseño Responsivo: Se adapta a diferentes tamaños de pantalla con una interfaz moderna y pulida.
Animaciones Suaves: Animaciones con suavizado cuadrático para movimientos naturales, con contornos en las piezas para mayor claridad visual.

Tecnologías Utilizadas

HTML5: Estructura de la aplicación web.
CSS3: Estilización con fondo degradado, animaciones en botones y diseño responsivo.
JavaScript: Lógica principal para la manipulación del cubo e interacciones del usuario.
Three.js (r134): Renderizado 3D del cubo con MeshStandardMaterial para iluminación y sombras realistas.
WebGL: Para renderizar la escena 3D en el navegador.

Instalación

Clonar o Descargar: Obtén los archivos del proyecto (por ejemplo, rubiks_cube.html).
Ejecutar Localmente:
Abre rubiks_cube.html en un navegador web moderno (Chrome, Firefox, Edge, etc.).
No se requiere configuración adicional, ya que Three.js se carga mediante CDN (https://cdnjs.cloudflare.com/ajax/libs/three.js/r134/three.min.js).

Servidor Web Opcional:
Para una mejor experiencia, sirve el archivo usando un servidor local (por ejemplo, python -m http.server o npx serve).
Accede a la aplicación en http://localhost:<puerto>.

Uso

Controles:
Botones: Haz clic en los botones etiquetados como U, U', D, D', L, L', R, R', F, F', B, B' para rotar las caras correspondientes (en sentido horario o antihorario).
Mezclar: Haz clic en el botón "Mezclar" para aplicar 20 movimientos aleatorios.
Reiniciar: Haz clic en el botón "Reiniciar" para restaurar el cubo a su estado resuelto.
Resolver: Haz clic en el botón "Resolver" para revertir la secuencia de mezcla y resolver el cubo.
Órbita: Haz clic y arrastra con el ratón para rotar todo el cubo y verlo desde diferentes ángulos.

Tutorial: Desplázate por la sección de tutorial en la parte inferior para seguir el método para principiantes, utilizando la notación estándar (por ejemplo, R' D' R D).

Estructura del Proyecto

rubiks_cube.html: Archivo principal que contiene HTML, CSS y JavaScript.
HTML: Define el lienzo para el renderizado 3D, los botones de control y la sección de tutorial.
CSS: Estiliza la interfaz con un fondo degradado, animaciones en botones y un diseño responsivo.
JavaScript: Implementa la lógica del cubo, incluyendo:
Inicialización del cubo con 26 piezas visibles (3x3x3 menos el centro).
Lógica de rotación de caras utilizando transformaciones en el sistema de coordenadas local.
Actualización de posiciones y materias para mantener la integridad del cubo.
Animaciones con suavizado cuadrático para rotaciones fluidas.
Funcionalidad de mezcla y resolución con cola de movimientos.

Limitaciones Conocidas

El botón "Resolver" revierte la secuencia de mezcla en lugar de resolver el cubo desde cualquier estado. Se podría implementar un algoritmo de resolución completo (por ejemplo, el algoritmo de Kociemba).
El rendimiento puede variar en dispositivos de baja potencia debido al renderizado WebGL.
No se han implementado controles por teclado; se podrían añadir para mejorar la accesibilidad.

Mejoras Futuras

Agregar atajos de teclado para los movimientos del cubo (por ejemplo, presionar 'U' para rotar la cara superior).
Implementar un algoritmo completo de resolución para cualquier estado del cubo.
Añadir controles táctiles para dispositivos móviles.
Incluir un contador de movimientos y temporizador para practicar speedcubing.
Mejorar la iluminación con mapas de entorno para una apariencia más realista del cubo.

Contribución
¡Las contribuciones son bienvenidas! Para contribuir:

Haz un fork del repositorio (si está alojado en una plataforma como GitHub).
Crea una rama para tu funcionalidad (git checkout -b nombre-funcionalidad).
Realiza los cambios y pruébalos exhaustivamente.
Envía un pull request con una descripción clara de los cambios.

Licencia
Este proyecto es de código abierto y está disponible bajo la Licencia MIT.
Acknowledge

Construido con Three.js para renderizado 3D.
Inspirado en la notación estándar del cubo de Rubik y el método de resolución para principiantes.
Diseñado para fines educativos y recreativos.
