# DOSW_Lab3_Tovar_Solano_Rodriguez_Botero
## Preguntas — Maven y Pull Requests

### 1. ¿Qué es un Maven Archetype?
Es una plantilla que genera automáticamente la estructura básica de un proyecto Maven (carpetas, `pom.xml` y archivos iniciales).

### 2. ¿Cuál es el propósito del archetype `maven-archetype-quickstart`?
Generar rápidamente la estructura mínima de un proyecto Java simple, con una clase principal y una clase de prueba de ejemplo.

### 3. ¿Qué comando se puede usar para crear un proyecto a partir de un archetype de Maven?
```bash
mvn archetype:generate \
  -DgroupId=edu.eci.dosw.lab \
  -DartifactId=DOSW-Laboratorio3 \
  -DarchetypeArtifactId=maven-archetype-quickstart \
  -DinteractiveMode=false
```

### 4. ¿Qué es un pull request en GitHub?
Es una solicitud para fusionar los cambios de una rama hacia otra, permitiendo que el equipo los revise y apruebe antes de integrarlos.

### 5. ¿Cómo se crea un pull request en GitHub?
Se sube la rama con los cambios, se va a la pestaña Pull requests, se hace clic en New pull request, se seleccionan la rama base y la rama a comparar, se agrega título y descripción, y se hace clic en Create pull request.

### 6. ¿Cómo se aprueba un pull request en GitHub?
Se entra al pull request, se revisan los cambios en Files changed, se hace clic en Review changes, se selecciona Approve y se hace clic en Submit review.

### Bibliografía

Apache Software Foundation. (2023). *Introduction to archetypes*. Apache Maven Project. https://maven.apache.org/guides/introduction/introduction-to-archetypes.html

Apache Software Foundation. (2023). *Maven archetype quickstart*. Apache Maven Project. https://maven.apache.org/archetypes/maven-archetype-quickstart/index.html

GitHub Docs. (2024). *About pull requests*. GitHub. https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests

GitHub Docs. (2024). *Reviewing proposed changes in a pull request*. GitHub. https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/reviewing-proposed-changes-in-a-pull-request
