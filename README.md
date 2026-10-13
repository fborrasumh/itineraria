# ItinerarIA

Seminarios de Historia de la Medicina y Antropología Médica con trabajo de campo simulado. Aplicación web de un solo fichero.

**Usar la app:** https://fborrasumh.github.io/itineraria/

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23352037.svg)](https://doi.org/10.5281/zenodo.23352037)

**Idiomas:** español (por defecto), inglés, portugués; selector en la barra superior (o `?lang=en` / `?lang=pt` en la URL).

## Qué hace

Acompaña a un grupo de estudiantes en la preparación de un seminario, en seis pasos:

1. **Seminario.** Elección del seminario (estigma y obesidad, medicalización, financiación sanitaria, especialización médica), la subcuestión y la pregunta del grupo.
2. **Trabajo de campo.** Entrevistas a pacientes simulados por IA con el guion del modelo explicativo de Kleinman y el itinerario terapéutico. Al terminar, comentarios formativos sin nota y métricas calculadas por código (preguntas, abiertas y cerradas, proporción de palabras del paciente, dimensiones exploradas).
3. **Análisis.** Temas con fragmentos de las transcripciones, comprobados por código, y una tabla de temas por entrevista. La IA puede sugerir temas, siempre con un fragmento literal, y el grupo decide.
4. **Informe.** Contador de palabras con la bibliografía incluida, comprobación de las citas numeradas y corrector de referencias en estilo NLM. Con PMID, DOI o título, la referencia correcta se reconstruye desde PubMed o Crossref y se compara campo a campo.
5. **Exposición.** Guion por bloques, suma de minutos, estimación del tiempo de habla y cronómetro de ensayo.
6. **Debate.** Un tribunal simulado (compañeros y profesor) pregunta a partir de frases del informe y comenta las respuestas.

Sección de **profesorado**: editar seminarios, criterios y límites; revisar y validar casos; pedir borradores de casos a la IA; exportar la actividad o generar una **página para el alumnado** que solo muestra los casos validados. Sección **Proyecto del grupo**: guardar y abrir el proyecto en JSON, dossier en Word y registro de uso de la IA (fecha, fase y modelo, nunca el contenido).

## Cómo se usa la IA

Con la propia clave de OpenAI, Google Gemini o Anthropic Claude. La clave se guarda solo en el navegador. No hace falta servidor.

## Privacidad

Todo el proyecto se guarda en el navegador (IndexedDB). Hacia el proveedor de IA solo salen el caso del paciente, las preguntas del grupo y el texto que se pide comentar, con los nombres de los miembros del grupo, correos, DNI y teléfonos enmascarados; antes del primer envío de cada sesión se muestra lo que sale y se pide confirmación. Al comprobar referencias, solo el PMID, el DOI o el título viajan a PubMed (NCBI E-utilities) o Crossref.

## Límites

- Los pacientes son **simulados**: sirven para entrenar la escucha y preparar el seminario, no son datos empíricos ni se citan como evidencia.
- Los ocho casos de serie son una propuesta inicial de los autores de la app y deben ser revisados y validados por el profesorado antes de usarse en clase.
- Los comentarios de la IA son orientativos y no sustituyen la evaluación del profesorado. Si la IA pone una nota, el código quita esa frase.
- El código comprueba que las citas de la IA aparezcan literalmente en el material, pero no puede comprobar si sus interpretaciones son acertadas.
- La clasificación de preguntas abiertas y cerradas es una estimación por cómo empieza cada pregunta.
- El corrector NLM cubre artículos de revista y libros; Crossref no siempre ofrece la abreviatura NLM de la revista.
- No hay servidor: el trabajo en grupo se comparte pasando el fichero del proyecto.

## Autoría

Fernando Borrás Rocher (Universidad Miguel Hernández de Elche) y Enrique Perdiguero Gil (Universidad Miguel Hernández de Elche).

Diseñada para los seminarios de la asignatura «Historia de la Medicina, Documentación y Antropología Médica» (Grado en Medicina, UMH): estigma y obesidad, medicalización, financiación sanitaria y especialización médica.

ORCID: Fernando Borrás Rocher [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573) · Enrique Perdiguero Gil [0000-0003-0870-3512](https://orcid.org/0000-0003-0870-3512)

## Cómo citar

Borrás Rocher, F. y Perdiguero Gil, E. (2026). *ItinerarIA* (v1.0.0) [Software]. DOI: [10.5281/zenodo.23352037](https://doi.org/10.5281/zenodo.23352037)

## Licencia

MIT. Véase [LICENSE](LICENSE).
