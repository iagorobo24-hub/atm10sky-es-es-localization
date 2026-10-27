# System Map — atm10sky-es-es-localization

**Estado:** `draft` · **Perfil provisional:** `LITE` · **Fecha:** 2026-10-27  
**HEAD de descubrimiento GitHub:** `main` @ `2ecb34d4f9969ad550e5eed4c9377fa785e29db2`  
**Alcance:** snapshot de rutas; no revisión de funcionamiento ni certificación arquitectónica.

## Catálogo de enrutamiento

| Fuente | Ruta | Alcance |
|---|---|---|
| `README.md` | [Abrir](../../README.md) | Localizado en el árbol GitHub; evidencia arquitectónica por determinar |
| `docs/system-map/manifest.yaml` | [Metadatos](./manifest.yaml) | Snapshot remoto y cobertura `unknown` |

## Why this shape

Se introduce un mapa mínimo para empezar sin inventar la arquitectura de este proyecto ni replicar documentación existente. Se ha comprobado la existencia de los documentos referenciados en el árbol Git de la rama anotada; no se ha verificado su contenido integral, código runtime o estado local. El `source.commit` es la referencia de descubrimiento remoto, **no una línea base validada**. Revisar si procede un perfil `FULL` durante el discovery.

## Impacto e invariantes

- Dominios, flujos, fronteras, invariantes: `UNKNOWN` (no modelados aún).
- **Hits / Does not hit:** por establecer antes de modificar arquitectura.
- Test execution: `NOT RUN`; despliegue, integraciones y dispositivos: `UNVERIFIED`.

## Ruta de validación pendiente

1. Descubrir gobernanza y código, reconciliar docs canónicas y confirmar responsabilidades y puntos de entrada.
2. Construir el mapa con rutas, símbolos, edges y excepciones demostradas y clasificar la evidencia.
3. Ejecutar validación mecánica, revisión semántica y Cold-Agent Walk; solo entonces convertir `draft` a `active`.

**Gates:** `MECHANICAL_GATE: UNAVAILABLE`, `SEMANTIC_AGENT_REVIEW: PENDING`. Toda afirmación de comportamiento requiere prueba específica.
