# Burney Relief (Queen of the Night) – 3D Model Processing

***

## Descripción

Este repositorio contiene el resultado de la práctica de procesado y publicación de un modelo 3D patrimonial, siguiendo los pasos indicados en la asignatura de Digitalización del Patrimonio Cultural (UNED).  
El modelo utilizado es **burney_relief_queen_of_the_night_draft**.  
El flujo de trabajo se ha realizado íntegramente con MeshLab y herramientas libres.

## Proceso seguido

1. **Importación del modelo:**  
   Se importó la nube de puntos original en MeshLab.

2. **Cálculo de normales:**  
   Se calcularon normales para la nube de puntos si era necesario.

3. **Triangulación:**  
   Se generó una malla de triángulos mediante el filtro *Screened Poisson*.

4. **Limpieza y reparación de topología:**  
   Se eliminaron caras y vértices duplicados, se cerraron agujeros y se corrigieron errores topológicos.

5. **Simplificación:**  
   La malla se redujo a menos de 10.000 triángulos usando *Quadric Edge Collapse Decimation*.

6. **Parametrización UV:**  
   Se aplicó *Parametrization: Trivial Per-Triangle* para asignar coordenadas de textura.

7. **Generación de textura:**  
   Se transfirió el color por vértice a una textura 2D con *Transfer: Vertex Attributes to Texture*.

8. **Exportación:**  
   Se exportó la malla final junto con la textura en formato compatible con visualización web.

9. **Publicación:**  
   Los archivos se subieron a este repositorio y se publicó el modelo en GitHub Pages mediante un visor X3Dom.

## Archivos incluidos

- `burney_relief_queen_of_the_night_draft.obj` / `.x3d` / `.ply`: Modelo 3D final simplificado y texturizado.
- `burney_relief_queen_of_the_night_draft.png` / `.jpg`: Textura generada.
- `burney_relief_queen_of_the_night_draft_original.xyz` / `.ply`: Nube de puntos original.
- `README.md`: Este documento.
- `index.html`: Archivo para visualización web del modelo.

## Visualización online

Puedes ver el modelo publicado en:  
[ENLACE_A_TU_GITHUB_PAGES]

## Créditos y licencia

- Modelo original proporcionado por la UNED para fines educativos.
- Procesado y documentación: Antonio Arquelladas Martínez
- Herramientas utilizadas: MeshLab, GitHub Pages.

***


