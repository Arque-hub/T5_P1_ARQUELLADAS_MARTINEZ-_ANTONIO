Práctica: Publicación de Modelo 3D "Mummy Mask" en la Web
Descripción
Este repositorio contiene el resultado de la práctica de digitalización, simplificación y publicación web del modelo 3D Mummy Mask. El objetivo ha sido transformar una nube de puntos densa en una malla ligera y texturizada, apta para su visualización interactiva en la web mediante X3Dom y GitHub Pages.

Modelo seleccionado
Nombre: Mummy Mask

Vértices originales: 255,979

Proceso seguido
1. Carga y Análisis Inicial
Importación del modelo original en MeshLab.

Verificación de atributos: número de vértices, presencia de color y normales.

2. Triangulación
Comprobación y cálculo de normales si era necesario.

Generación de la malla de triángulos usando el filtro Surface Reconstruction: Screened Poisson (profundidad 10).

Visualización y captura del resultado de la triangulación, mostrando claramente la estructura de triángulos (“Show Faces” y “Show Wireframe”).

3. Limpieza y Reparación Topológica
Eliminación de triángulos artificiales con el filtro Select Faces with edges longer than....

Aplicación de filtros de selección para detectar y borrar errores topológicos: caras autointersectadas, aristas y vértices non-manifold, componentes desconectados.

Cierre progresivo de fisuras con el filtro Close Holes.

4. Simplificación de la Malla
Duplicado de la malla antes de simplificar.

Reducción de la malla a menos de 10,000 vértices con el filtro Quadric Edge Collapse Decimation.

Nueva comprobación y reparación de errores topológicos.

5. Parametrización y Texturizado
Generación de coordenadas de textura con Parametrization: Voronoi Atlas.

Transferencia del color por vértice de la malla original a textura mediante Transfer: Vertex Attributes to Texture.

Asignación y comprobación de la textura sobre la malla simplificada.

6. Exportación y Publicación
Exportación de la malla final en formato X3D, asegurando la correcta inclusión de normales y coordenadas de textura.

Revisión de nombres de archivos y carpetas (sin espacios, tildes ni caracteres especiales).

Creación de la página web con X3Dom y subida de todos los archivos al repositorio.

Configuración de GitHub Pages para la publicación online.

## Créditos y licencia

- Modelo original proporcionado por la UNED para fines educativos.
- Procesado y documentación: Antonio Arquelladas Martínez
- Herramientas utilizadas: MeshLab, GitHub Pages.

***


