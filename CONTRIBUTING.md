# Cómo se trabaja en los repositorios de la organización

Los repositorios de `Ecosistema-Uthgra-CABA` son propiedad de UTHGRA Seccional CABA desde el primer día (art. 18.1 del Pliego Consolidado v2.0). El proveedor adjudicatario trabaja sobre ellos con acceso de escritura a las ramas de desarrollo.

## Ramas (art. 18.1)

| Pliego | Rama | Regla |
|---|---|---|
| Producción | `main` | Solo por pull request con aprobación de UTHGRA CABA |
| Integración | `develop` | Pull request con revisión |
| Funcionalidades | `feature/<hito>-<descripcion>` | Libre para el proveedor; se integra a `develop` por pull request |
| Correcciones urgentes | `hotfix/<descripcion>` | Sale de `main` y vuelve a `main` y `develop` por pull request |

## Reglas

- **Actualización diaria.** Desde H1 el repositorio se mantiene activo con actualización diaria. El código no puede residir solo en infraestructura del proveedor (art. 18.1).
- **Todo cambio entra por pull request**, usando la plantilla del repositorio.
- **Prohibido** el código ofuscado, los binarios sin fuente y las dependencias de repositorios privados no auditados.
- **Nunca** se suben credenciales, secretos ni datos personales reales.
- **Idioma:** documentación, issues y pull requests en español.
- **Entregas de hito:** se notifican con un issue "Entrega de hito". La fecha de ese issue inicia los 10 días hábiles de revisión (art. 3.2).
- **Pliego y simulador.** En el repositorio del sistema, las carpetas `pliego/`, `simulador/`, `legal/`) contienen documentos de UTHGRA CABA: no se modifican por pull request del proveedor; sus huellas están en `INTEGRIDAD.md`.
