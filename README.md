# NarrativIA

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21949740.svg)](https://doi.org/10.5281/zenodo.21949740)

**Aplicación:** https://fborrasumh.github.io/narrativia/

Convierte las salidas de un **cuaderno Jupyter ejecutado** en la **sección de Resultados** de un artículo. Cada frase queda enlazada con los hallazgos que la respaldan, así que se puede comprobar no solo que una cifra existe, sino que pertenece al resultado del que habla. Aplicación de un solo fichero, sin servidor.

## Novedades de la versión 3.0

- **Interfaz en español, inglés y portugués**, con selector. El texto del manuscrito tiene su propio idioma (español, inglés, valenciano/catalán o portugués), con sus etiquetas de tabla y figura.
- **Proveedores de IA en la nube con tu propia clave:** OpenAI, Google Gemini y Anthropic Claude, con desplegable de los modelos de tu clave. **Se elimina la opción local con Ollama.**
- **Ejemplo sin clave:** el cuaderno de dietas funciona en los tres idiomas con una respuesta de IA precalculada que pasa por las mismas comprobaciones (incluye a propósito tres fallos que se detectan y se corrigen). Las versiones en inglés y portugués traducen solo las etiquetas; la figura conserva sus etiquetas en español.
- **Aviso previo al envío** con muestra de lo que sale y datos personales (correos, DNI, teléfonos) enmascarados. Las figuras no se pueden enmascarar y se avisa.
- **Word sin librerías externas** (también con la figura incrustada), además de Markdown, texto e informe de revisión.
- **Verificador de cifras mejorado:** ya no marca plazos como «a los 6 meses» y entiende la coma decimal («1,575»). Reconoce «tendencia a la significación», interpretación y lenguaje causal también en inglés y portugués.
- Los proyectos guardados con la v2.0 siguen disponibles.

## Cómo funciona

Analista de evidencia (IA) → contraste de la ficha con las salidas (código) → redactor (IA) → verificador de cifras (código) → revisor conceptual (IA) → corrector (IA) → verificación final (código).

## Privacidad y límites

El cuaderno se lee en el navegador; al proveedor solo se envían las salidas que marques, con los datos personales enmascarados y tras un aviso previo. La clave se guarda solo en tu navegador y los proyectos en IndexedDB. La verificación automática reduce errores, no los elimina: no sabe si el análisis estadístico del cuaderno era el adecuado. Revisa el texto antes de enviarlo. Probada con IA simulada; no se ha probado con claves reales de cada proveedor.

## Cómo citar

Borrás Rocher, F. (2026). *NarrativIA* (versión 3.0.0) [Software]. Universidad Miguel Hernández de Elche. https://doi.org/10.5281/zenodo.21949740

El DOI es el de concepto: apunta siempre a la última versión. GitHub ofrece la cita con el botón *Cite this repository*, a partir de `CITATION.cff`.

Forma parte del catálogo [Herramientas IA para la academia](https://fborrasumh.github.io/ia/).

## Licencia

MIT © 2026 Fernando Borrás Rocher · Universidad Miguel Hernández de Elche.
