# SPEC-000 – Foundation

## 1. Propósito

Establecer las bases técnicas, organizativas y de desarrollo de TaskFlow Lite para mantener un proyecto simple, consistente y fácil de evolucionar.

Esta especificación define las tecnologías, estructura inicial, convenciones y criterios técnicos mínimos que deberán cumplirse antes de comenzar con la implementación de funcionalidades.

## 2. Alcance

Esta SPEC establece:

* Las tecnologías permitidas para TaskFlow Lite.
* La estructura inicial de archivos y directorios.
* Las restricciones técnicas del proyecto.
* Las convenciones de nombres utilizadas en archivos, variables y funciones.
* Las convenciones básicas para el uso de Git.
* La definición inicial de terminado técnico.
* Los elementos que permanecerán fuera del alcance en esta etapa.

No define funcionalidades de negocio ni historias de usuario.

## 3. Estructura inicial del proyecto

El código fuente del proyecto se organizará dentro del directorio `src/`.

La estructura inicial será:

```text
TaskFlow-Lite/
├── src/
│   ├── index.html
│   ├── css/
│   └── js/
├── SPEC-000-foundation.md
└── README.md
```

La estructura podrá crecer de forma incremental conforme se agreguen nuevas especificaciones e historias, sin incorporar elementos que no sean necesarios para el objetivo correspondiente.

## 4. Restricciones técnicas

TaskFlow Lite deberá cumplir las siguientes restricciones:

* Utilizar **HTML5** para la estructura de las interfaces.
* Utilizar **CSS3** para presentación y estilos.
* Utilizar **JavaScript ES Modules** para la lógica del cliente.
* No utilizar frameworks de frontend o backend.
* No utilizar backend, servidor de aplicaciones ni API propia.
* La persistencia de información deberá contemplar **`localStorage`** como mecanismo futuro.
* El proyecto deberá poder desarrollarse y ejecutarse desde **VSCode**.
* El código fuente deberá permanecer organizado dentro de `src/`.
* No se implementarán historias funcionales en esta SPEC.

## 5. Convenciones de nombres

Para mantener consistencia en el código se utilizarán las siguientes convenciones:

### Archivos y directorios

* Directorios: nombres en minúsculas.
* Archivos HTML y CSS: nombres en minúsculas utilizando `kebab-case` cuando sea necesario separar palabras.
* Archivos JavaScript: nombres en minúsculas utilizando `kebab-case`.

### JavaScript

* Variables y funciones: `camelCase`.
* Constantes: `UPPER_SNAKE_CASE` cuando representen valores constantes globales.
* Clases: `PascalCase`.
* Los nombres deberán describir claramente la responsabilidad del elemento.

### HTML y CSS

* Los identificadores (`id`) utilizarán nombres descriptivos.
* Las clases CSS utilizarán `kebab-case`.
* Se evitarán nombres genéricos que no indiquen claramente su propósito.

## 6. Convenciones de Git

El repositorio deberá utilizar Git para controlar las versiones del proyecto.

Se establecen las siguientes convenciones iniciales:

* Cada cambio deberá registrarse mediante commits pequeños y relacionados con una sola modificación lógica.
* Los mensajes de commit deberán describir claramente el cambio realizado.
* Se recomienda utilizar el formato:

```text
tipo: descripción breve
```

Tipos permitidos inicialmente:

* `feat`: nueva funcionalidad.
* `fix`: corrección de errores.
* `docs`: documentación.
* `refactor`: reorganización del código sin cambiar su comportamiento.
* `style`: cambios de formato o estilos.
* `chore`: tareas de mantenimiento.

Ejemplo:

```text
docs: agrega SPEC-000 de fundación
```

## 7. Definition of Done técnica inicial

La fundación técnica se considerará terminada cuando:

* La estructura inicial del proyecto exista y esté organizada dentro de `src/`.
* Se hayan definido y respetado las tecnologías establecidas.
* No existan frameworks ni backend dentro del proyecto.
* Los archivos utilicen las convenciones de nombres establecidas.
* El proyecto pueda abrirse y ejecutarse desde VSCode.
* El repositorio Git esté inicializado y permita registrar cambios mediante commits.
* La presente especificación esté almacenada como `SPEC-000-foundation.md`.
* No se hayan implementado historias funcionales como parte de esta SPEC.

## 8. Fuera de alcance

Quedan fuera del alcance de esta SPEC:

* Registro, edición, eliminación o consulta de tareas.
* Estados o prioridades de tareas.
* Búsqueda o filtrado de tareas.
* Diseño funcional de las interfaces.
* Persistencia funcional mediante `localStorage`.
* Autenticación o gestión de usuarios.
* Backend, APIs o bases de datos.
* Frameworks o librerías de frontend.
* Historias de usuario y criterios de aceptación.
* Implementación de funcionalidades de negocio.
