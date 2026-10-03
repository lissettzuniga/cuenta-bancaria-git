# Cuenta bancaria — Git y pull requests

**Autor:** Lissett Zuñiga Reyes

## Cómo correr

    ./correr.sh

## Mis pull requests

| # | Qué cambió |
|---|---|
| 1 | El estado de cuenta muestra cuántos retiros se hicieron y cuántos fueron gratis |
| 2 | README y evidencia de la práctica |

## Boleto de salida

1. ¿Qué diferencia hay entre `git add` y `git commit`?

   `git add` mueve los cambios del directorio de trabajo al área de preparación (staging area), seleccionando lo que se guardará. `git commit` toma lo que está en el área de preparación y lo guarda permanentemente en la historia del repositorio con un mensaje explicativo.

2. ¿Por qué después del merge en GitHub tu `main` de Ubuntu no tenía el cambio hasta que hiciste `git pull`?

    Porque el merge ocurrió de forma remota en los servidores de GitHub. Mi copia local en Ubuntu no sincroniza automáticamente la historia con internet; necesité ejecutar `git pull` para descargar e integrar los commits nuevos a mi máquina.

3. Abriste un PR y después hiciste otro commit en la misma rama. ¿Qué pasó con el PR?

   El PR se actualizó automáticamente incluyendo el nuevo commit. Esto sucede porque un Pull Request está vinculado al historial completo de la rama compare, no solo a la foto del momento en que se creó.

4. ¿Por qué en un equipo nadie hace cambios directamente en `main`?

   Para proteger la rama principal de errores, código incompleto o fallos en producción. Trabajar en ramas permite revisar, probar y discutir el código mediante Pull Requests antes de integrarlo de forma segura a `main`.