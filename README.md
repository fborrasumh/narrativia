# NarrativIA

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21949740.svg)](https://doi.org/10.5281/zenodo.21949740)

**Aplicación:** https://fborrasumh.github.io/narrativia/

Convierte las salidas de un **cuaderno Jupyter ejecutado** en la **sección de Resultados** de un artículo. Cada frase queda enlazada con los hallazgos que la respaldan, así que se puede comprobar no solo que una cifra existe, sino que pertenece al resultado del que habla. Aplicación de un solo fichero, sin servidor.

## Novedades de la versión 2.0

- Interfaz guiada con el estilo de Forja y un cuaderno de ejemplo real, ejecutado con Python.
- **Ficha de hallazgos**: un agente extrae prueba, grupos, estadístico, p, IC, tamaño del efecto y n. Cada valor se busca en su salida original y lo que no aparece queda marcado como «NO USAR».
- **Redacción frase a frase con citas** a los hallazgos.
- **Verificador de cifras sin IA**: clasifica cada número como respaldado, atribuido a otro resultado o sin respaldo. Además marca «tendencia a la significación», «p = 0,000», el lenguaje interpretativo, la causalidad en diseños observacionales, tablas o figuras sin citar y hallazgos principales omitidos.
- **Revisor conceptual y corrector**: detectan la ausencia de evidencia tratada como ausencia de efecto, la dirección invertida y la confusión entre resultados ajustados y sin ajustar. Solo se reescriben las frases señaladas, y todo se verifica de nuevo.
- **Integración con CuadernIA 2.0**: lee el diseño, el α y la verificación del cuaderno.
- **Corregido**: los valores p en formato APA («p = .034») ya no se marcan como cifras sin respaldo.

## Privacidad

El cuaderno se lee en el navegador; al modelo solo se envían las salidas que marques. Funciona con OpenAI (clave en `localStorage`, `ia_openai_key`) o con un modelo local mediante Ollama. Los proyectos se guardan en IndexedDB.

## Cómo citar

Borrás Rocher, F. (2026). *NarrativIA* (versión 2.0.0) [Software]. Universidad Miguel Hernández de Elche. https://doi.org/10.5281/zenodo.21949740

El DOI anterior es el de concepto: apunta siempre a la última versión. El DOI de cada versión concreta está en [Zenodo](https://doi.org/10.5281/zenodo.21949740). GitHub ofrece la cita en formato APA y BibTeX con el botón *Cite this repository*, a partir de `CITATION.cff`.

Forma parte del catálogo [Herramientas IA para la academia](https://fborrasumh.github.io/ia/).

## Licencia

MIT © 2026 Fernando Borrás Rocher · Universidad Miguel Hernández de Elche.
