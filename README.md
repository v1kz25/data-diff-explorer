# data-diff-explorer

> Estado: planificación inicial. **Aún no hay MVP implementado**.

Aplicación de escritorio read-only para comparar datasets CSV/Parquet y tablas SQLite/DuckDB.

## Objetivo

Identificar cambios de esquema, registros y calidad entre dos conjuntos de datos locales sin alterar los originales.

## Stack provisional

C#/.NET + Avalonia + DuckDB.NET (validar versiones, licencia del toolkit y distribución). La versión concreta y la idoneidad se validarán en el primer spike técnico.

## MVP previsto

- abrir localmente CSV/Parquet y tablas SQLite/DuckDB
- seleccionar claves y comparar esquemas
- detectar filas añadidas, eliminadas o modificadas
- navegar diferencias paginadas y exportar un reporte

### Fuera del MVP

- edición de datos
- cliente SQL general
- conexiones remotas y servidores
- LLM/servicios de pago
- cargar datasets completos en memoria

## Desarrollo

- Ver [roadmap](docs/ROADMAP.md), [guía de desarrollo](docs/DEVELOPMENT.md) y [AGENTS.md](AGENTS.md).
- El punto de entrada son los GitHub Issues, no implementar el MVP de golpe.
- Desarrollo principalmente desde Windows 11; sin infraestructura de pago.

## Riesgos

Escalabilidad, colisiones en keys, semántica NULL/NaN/timestamp, tipos anidados de Parquet, distribución de UI Avalonia.

## Referencias

- https://duckdb.org/
- https://github.com/l1xnan/duckling
- https://github.com/antonycourtney/tad

## Licencia

**Pendiente de decisión.** Este repositorio se publica sin archivo LICENSE por ahora. Ser público en GitHub no otorga automáticamente permiso para copiar, modificar o redistribuir su contenido.
