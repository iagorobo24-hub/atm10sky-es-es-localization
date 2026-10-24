# Informe técnico — Traducción es_es de FTB Quests en ATM10: To the Sky v2.0.7

**Revisión del informe:** 2026-10-24 (corrige la versión anterior, que contenía afirmaciones no respaldadas; ver §8)  
**Modpack:** *All the Mods 10: To the Sky v2.0.7* (Minecraft 1.21.1, NeoForge, 349 mods)  
**Candidata publicada:** `es_es_EDITORIAL_191_FIEL_AL_EN_NO_ACTIVAR.snbt` → `es_es.snbt` en este repositorio  
**SHA-256 de la candidata 191:** `276dc8389226097fc726d77a5d9412f339277518ec23417a6eefa48044868209`  
**SHA-256 del `es_es.snbt` original de CurseForge:** `41d3cf485987b137b6611cee5cd48043d0ed69237c0772e4eb55bf6496308f66`

Este documento separa con claridad **lo comprobado** de **lo no comprobado**.

---

## 1. Resumen

| Concepto | Valor | Cómo se obtuvo |
|---|---|---|
| Claves del inglés (`en_us.snbt`) | 6.462 | Recuento directo |
| Claves ausentes frente al inglés | **0** | Comparación automática de claves |
| Errores de parseo SNBT, comillas, macros e imágenes | **0** | Validador propio (`lang_tools.py`) |
| Firmas de color / saltos de línea rotas (`broken_signature`) | **0** | Validador propio |
| Descripciones rehechas desde el inglés | **189** | 53 (B01) + 80 (B02) + 22 (B09) + 1 (título de tarea) + 33 (candidata 191) |
| Claves «solo-ES» conservadas | **137** | 69 títulos + 68 descripciones sin equivalente en inglés |
| Revisión visual en el juego | **Muestreo** | Ver §4 |

Las cifras de la versión anterior de este informe que **no** se mantienen: «812 nombres en inglés justificados», «0 prosa inglesa residual» como garantía, «0 errores en el log en la 191», «83/83 lotes aprobados visualmente». Ver §3 y §8.

---

## 2. Cadena de candidatas

Cada candidata se construyó a partir de la anterior y se validó estáticamente antes de pasar a la siguiente.

1. **183** — añadió las 144 claves que faltaban frente al inglés (`missing_vs_en = 0`).
2. **184** — correcciones de estilo y puntuación.
3. **185** — traducción de 107 claves traducibles dispersas (licencias, tablas de recompensa, títulos genéricos).
4. **186** — localización de 18 descripciones que seguían en inglés.
5. **187** — unificación de «fabricar» en lugar de «craftear» (39 claves).
6. **188** — reescritura desde el inglés de 53 descripciones de la sección Progresión.
7. **189** — reescritura de 80 descripciones de la sección Fundamentos.
8. **190** — reescritura de 22 claves de Equipo y Combate más un título de tarea; `broken_signature` llegó a 0. Es la candidata de la que existe muestreo en el juego (§4).
9. **191** — reescritura de 33 descripciones con glosas JEI/EMI añadidas o comentarios meta, y unificación de «Mesa de Reforjado» / «Mesa de Reforjado Simple» y «Matriz de Inducción». **Es la publicada aquí.**

---

## 3. Qué significa «83 lotes»

El trabajo se organizó internamente en 83 lotes agrupados en 9 bloques. El registro (`LOTES_ESTADO_191.json` y `.csv`) marca todos como aprobados, pero hay que leerlo con cautela:

- La aprobación se basa en **criterios estáticos** (claves presentes, firmas sin romper, sin prosa inglesa detectada por un escáner heurístico, nombres revisados) **más el muestreo** de §4. **No** implica que cada lote se haya abierto y revisado visualmente en el juego.
- Los totales por bloque **no son coherentes entre sí**: la suma de `claves_en` en el JSON no coincide con la de la tabla de la versión anterior de este informe ni con las 6.462 claves reales. Por eso esa tabla se ha eliminado. No usar estos ficheros como cifra oficial.

---

## 4. Revisión en el juego

**Realizado:**
- Se ejecutó un cliente de prueba con los 349 mods y se revisaron unas **25 pantallas** de la candidata **190** (capítulos y ventanas de misión), sin errores de FTB Quests en el registro durante esa sesión.
- Las capturas de `screenshots/` proceden de sesiones de prueba de las candidatas 183–190.

**No realizado / no demostrado:**
- Las **38 claves cambiadas en la 191** no se comprobaron una a una en el juego. La versión anterior de este informe describía una verificación visual de esas claves con capturas `qa191_*.jpg`; esas capturas **no existen** en el repositorio ni se conservaron, así que esa afirmación se retira.
- No se abrieron una a una las 3.753 misiones. La integridad del resto se apoya únicamente en la validación estática.

---

## 5. Terminología

Criterio: si el JAR del mod incluye `es_es.json` con un nombre oficial distinto del inglés, se usa ese nombre; si no, se conserva el inglés tal como aparece en JEI. No se inventan nombres.

Ejemplos comprobados contra los JAR de los mods:

- **Apotheosis:** Mesa de Reforjado, Mesa de Reforjado Simple.
- **Ars Nouveau:** Libreta Gastada.
- **Immersive Engineering:** Pararrayos.
- **Productive Bees:** Abeja carpintero verde, Abeja carpintero amarilla.
- **Mekanism:** Cubo de Energía, Cable Universal, Tubo Presurizado, Transportador Logístico, Tubería Mecánica, Entrelazoportador Cuántico, Configurador, Matriz de Inducción.

Mods cuyos nombres se mantienen en inglés porque no se encontró localización oficial en español en su JAR (según la revisión realizada; no es una lista cerrada auditada): Modern Industrialization, PneumaticCraft, XyCraft, LaserIO, Flux Networks, Integrated Dynamics, Transfer Labels, Dyson Cube Project, Just Dire Things.

Decisiones de estilo: `AllRightsReserved` → `TodosLosDerechosReservados`; «Bypass Trick» → «Truco para Saltárselo»; «craftear» → «fabricar».

---

## 6. Limitaciones

1. **Muestreo, no revisión completa.** Ver §4.
2. **Prosa inglesa residual.** Se buscó con un detector heurístico (marcas como «Objetivo:», «JEI/EMI», «texto original», proporción de longitud, números ausentes). Detecta bien los casos conocidos, pero `broken_signature = 0` **no** detecta una paráfrasis que casualmente conserve los mismos colores. No es una garantía formal.
3. **137 guías «solo-ES».** Son textos de los autores originales (67 de las descripciones contienen «Objetivo:») sin equivalente en inglés. Se conservan a propósito para no privar al jugador de esas explicaciones; implican que `es_es.snbt` no es una traducción estrictamente literal del inglés.
4. **Artefacto de renderizado.** En algunas ventanas de misión, la «í» de la primera línea puede verse sin tilde en pantalla aunque el archivo la contiene.
5. **Imágenes con texto en inglés.** Algunas cabeceras (p. ej. «Chapter 2: The Cool Parts», «Chapter 4: The ATM Star») tienen el texto dentro de la imagen del pack y no se pueden traducir desde el archivo de idioma.
6. **Sin revisión del equipo de ATM.** Es una contribución comunitaria no afiliada ni aprobada por All The Mods.

---

## 7. Estado de la instalación

- La candidata 191 está instalada en la instancia local del autor (`config/ftbquests/quests/lang/es_es.snbt`), con una copia de seguridad del original (`41d3cf48…`).
- Existe además una copia de seguridad de la 191 y del original fuera de la instancia.
- La versión anterior de este informe afirmaba que la instancia real estaba «100 % intacta» y que existía una réplica verificada en otro equipo; ninguna de las dos cosas es cierta o vigente (la 191 sí está instalada; la réplica ya no existe).

---

## 8. Correcciones respecto a la versión anterior

Se corrigieron o retiraron estas afirmaciones por no estar respaldadas:

| Afirmación anterior | Corrección |
|---|---|
| «QA visual in-game 83/83 lotes aprobados» | Aprobación por criterios estáticos más muestreo; no es revisión visual por lote |
| Tabla por bloques que sumaba 6.462 | Eliminada: los totales de los ficheros de lotes son inconsistentes |
| «QA visual in-game de las 38 claves de la 191» con capturas `qa191_*` | No comprobado; capturas inexistentes |
| «812 nombres en inglés justificados» | Cifra sin respaldo; retirada |
| «0 errores en el log de FTB Quests» (en la 191) | Solo observado en la sesión de la 190 |
| «Prosa inglesa residual: 0» | Resultado de un detector heurístico, no garantía |
| «Todas las capturas son de la candidata final» | Son de sesiones de las candidatas 183–190 |
| «Instancia real 100 % intacta; no se instaló nada» | Falso: la 191 está instalada, con copia de seguridad |
| «Réplica de seguridad verificada en otro equipo» | Ya no existe |
| Hallazgo sobre «Foundry Walls (Productive Metalworks / Dyenamics)» | Atribución no verificada; retirada |
| Propuesta de «pipeline automatizado multi-idioma para todos los modpacks ATM» | Retirada: no está demostrada |
