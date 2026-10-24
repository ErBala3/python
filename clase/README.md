# Mi clase · 2DAM

Web de la clase: <https://SergioJimenezDelOjo.github.io/python/clase/>

- **Horario** semanal con navegación entre semanas. Si una asignatura tiene tareas para esa semana, su cuadro lo marca: `N pendientes` en las clases anteriores a la entrega y `Entrega` el día que la tarea vence.
- **Ahora**: tarjeta con la clase en curso y los minutos que le quedan (o la siguiente). La clase actual se resalta en el horario con una barra de progreso y las que ya han pasado se atenúan.
- **Fin de semana**: el sábado y el domingo el horario, las entregas, el contador y la lista de tareas pasan a la semana que viene, para no ver lo de la semana ya terminada. También cambia solo la semana que toca en cada apartado.
- **Tareas** compartidas: lo que añade cualquiera aparece al momento para toda la clase. Cada uno marca como hechas las suyas, y también se pueden añadir tareas que solo salen en tu lista.
- **Ejercicios** por asignatura: se pueden pegar o subir archivos de código, verlos con colores, copiarlos, descargarlos y actualizarlos.
- **Cambiar asignaturas**: nombre, profesor/a, color y horario, para toda la clase.
- **Inicio de sesión** de la clase: hace falta para crear o modificar cosas. Para ver no hace falta.

Para probar sin tocar los datos reales, abre la página con `?demo` (por ejemplo `clase/?demo`). En ese modo todo se guarda solo en tu navegador.

## Datos (Firestore, proyecto `dam-calendario`)

| Ruta | Contenido |
| --- | --- |
| `Clase/2DAM` | Asignaturas, orden y horario (`horario.d0` … `horario.d4`, seis horas por día) |
| `Clase/2DAM/Tareas/{id}` | `titulo`, `asig`, `fecha` (AAAA-MM-DD), `tipo` (`clase` / `personal`), `desc`, `autor`, `hechas` (usuario → fecha) |
| `Clase/2DAM/Usuarios/{usuario}` | `nombre`, `sal`, `hash` (PBKDF2-SHA256), `iter` |
| `Codigo/Codigos/Archivos/{id}` | Ejercicios en la carpeta `2DAM/<SIGLA>`. Es la misma colección que usan `index.html` y SergioJimenezDelOjo/DAM, así que también aparecen allí |

**Seguridad:** igual que `index.html` y SergioJimenezDelOjo/DAM, la página entra en Firestore sin Firebase Authentication, con la configuración pública. Por eso el inicio de sesión sirve para saber quién eres y no para bloquear el acceso.
