<!-- Reemplaza todo lo que está entre {{ }} y adapta los comandos a tu proyecto. -->
# Cómo contribuir a {{nombre-proyecto}}

¡Gracias por tu interés! Esta guía explica cómo proponer cambios de forma que podamos revisarlos rápido.
Al participar aceptas nuestro [Código de Conducta](CODE_OF_CONDUCT.md).

## Formas de ayudar
- 🐛 **Reportar errores**: abre un issue con la plantilla "Reporte de error".
- 💡 **Proponer mejoras**: usa la plantilla "Solicitud de funcionalidad" y explica el problema antes que la solución.
- 📖 **Mejorar la documentación**: los arreglos de erratas pueden ir directo en un pull request.
- 🔧 **Escribir código**: busca issues con la etiqueta [`buen primer issue`]({{https://github.com/usuario/repo/labels/buen%20primer%20issue}}).

¿Vulnerabilidad de seguridad? **No abras un issue público**: sigue [SECURITY.md](SECURITY.md).

## Antes de escribir código
Para cambios grandes (nuevas funcionalidades, cambios de API, refactors amplios) **abre primero un issue** para acordar el enfoque. Así no inviertes tiempo en algo que no se pueda aceptar.

## Entorno de desarrollo
```bash
git clone https://github.com/{{tu-usuario}}/{{repo}}.git   # tu fork
cd {{repo}}
{{npm install}}
{{npm test}}        # todo debe pasar antes de empezar
```
Requisitos: {{Node.js ≥ 20}}.

## Flujo de trabajo
1. Crea una rama desde `{{main}}`: `git switch -c fix/descripcion-corta`.
2. Haz cambios pequeños y enfocados (un PR = un propósito).
3. Añade o actualiza tests para el comportamiento que cambias.
4. Ejecuta las verificaciones:
   ```bash
   {{npm run lint}}
   {{npm test}}
   ```
5. Actualiza la documentación y añade una entrada en `CHANGELOG.md` bajo `[Unreleased]` si el cambio es visible para usuarios.
6. Abre el pull request y completa la plantilla.

## Mensajes de commit
Usamos [Conventional Commits](https://www.conventionalcommits.org/es/v1.0.0/):
```
feat(parser): admite fechas con zona horaria
fix: evita división por cero en el resumen
docs: corrige el ejemplo de instalación
```
Tipos habituales: `feat`, `fix`, `docs`, `refactor`, `test`, `chore`. Un `!` (`feat!:`) indica un cambio incompatible.

## Estilo de código
- El formato lo aplica {{Prettier / ruff / gofmt}}: ejecuta `{{npm run format}}`.
- Nombres descriptivos; comentarios para explicar el *porqué*, no el *qué*.
- Sin dependencias nuevas sin comentarlo antes en el issue.

## Revisión
- Un mantenedor revisará tu PR en {{una semana}} aproximadamente.
- Es normal que pidamos cambios: no es nada personal, buscamos mantener el proyecto coherente.
- Si el PR queda inactivo {{30 días}} tras una petición de cambios, podemos cerrarlo (podrás reabrirlo).

## Licencia
Al contribuir aceptas que tu aporte se publique bajo la [licencia del proyecto](LICENSE).
