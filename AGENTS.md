# AGENTS.md

## Comunicación y continuidad

- Cuando el usuario autorice continuar en automático, avanzar dentro del alcance autorizado sin detenerse tras cada subtarea ni volver a pedir el mismo permiso.
- Al detenerse porque el trabajo terminó, existe un bloqueo o hace falta una decisión, explicar el resultado o bloqueo y ofrecer 2–3 próximos pasos concretos cuando haya alternativas útiles. Recomendar uno y explicar brevemente por qué; no cerrar solo con un informe de estado o una oferta genérica de ayuda.
- Mantener las opciones dentro de la autorización existente o señalar cuáles requieren una nueva decisión. No inventar trabajo innecesario para ofrecer opciones.

## Integración y limpieza al cerrar trabajo

- El cierre de un trabajo autorizado incluye integrar, actualizar su seguimiento y limpiar sus ramas y worktrees. Esta es una autorización permanente del usuario para los commits, publicación de la rama de trabajo, PR, merge y limpieza necesarios para ese cierre, salvo una restricción posterior explícita. No extenderla a trabajo ajeno, despliegues, datos ni servicios reales.
- Cuando el trabajo de un issue, PR, rama o worktree esté terminado, revisado y haya pasado las comprobaciones aplicables, integrar sus cambios en la rama de destino mediante el flujo del repositorio. No dejar trabajo terminado pendiente de merge por rutina ni volver a pedir una autorización ya concedida. Respetar protecciones y revisiones obligatorias; no eludirlas.
- Antes del merge, actualizar las referencias remotas y comprobar el diff, los commits y la evidencia de pruebas: confirmar que el contenido no esté ya integrado ni sustituido y que la validación corresponda al código que se integra. Resolver y volver a validar los cambios necesarios; si falta una comprobación requerida, clasificar el trabajo como pendiente o bloqueado, no como terminado.
- Tras el merge, verificar la integración contra el remoto, cerrar únicamente los issues cuyo alcance esté satisfecho y actualizar el seguimiento existente con la evidencia. Eliminar las ramas locales/remotas y los worktrees de ese trabajo solo tras confirmar que están integrados, que los worktrees están limpios y que no conservan contenido único ni están en uso por otra sesión. No borrar ramas protegidas ni trabajo ajeno.
- Si no puede integrarse o limpiarse algo, clasificarlo en el seguimiento existente como WIP, bloqueado, pendiente de validación, sustituido o integrado pendiente de limpieza, indicando motivo y siguiente acción. Conservar cambios sin commit y contenido único; no usar borrados forzados para ocultarlos ni crear inventarios duplicados.
- La integración, la limpieza o la clasificación explícita forman parte de la misma tarea. No acumular deuda de limpieza ni posponerla sin motivo: al cerrar, informar qué se integró, qué se eliminó y qué se conserva y por qué.
