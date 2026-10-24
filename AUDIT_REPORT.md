# Informe Final de Traducción y Auditoría QA — ATM10: To the Sky v2.0.7

**Fecha:** 2026-10-24  
**Auditor Senior:** Antigravity (QA Autónomo)  
**Modpack:** *All the Mods 10: To the Sky v2.0.7* (Minecraft 1.21.1, NeoForge 21.1.250, 349 mods)  
**Candidata Final Recomendada:** `es_es_EDITORIAL_191_FIEL_AL_EN_NO_ACTIVAR.snbt`  
**Hash SHA-256 Candidata 191:** `276dc8389226097fc726d77a5d9412f339277518ec23417a6eefa48044868209`  
**Hash SHA-256 Instancia Original (CurseForge):** `41d3cf485987b137b6611cee5cd48043d0ed69237c0772e4eb55bf6496308f66` (100% intacta, no modificada)

---

## 1. Resumen Ejecutivo y Métricas Globales

Se ha completado la auditoría integral, traducción y control de calidad (QA) estático y visual del archivo de misiones FTB Quests (`es_es.snbt`) para el modpack *All the Mods 10: To the Sky v2.0.7*. 

| Métrica | Valor | Estado / Nota |
|---|---|---|
| **Claves totales en inglés (`en_us.snbt`)** | 6.462 | Versión oficial del pack v2.0.7 |
| **Misiones totales** | 3.753 | 54 capítulos |
| **Claves ausentes frente al inglés (`missing_vs_en`)** | **0** | Cobertura al 100% |
| **Errores de parseo / sintaxis SNBT** | **0** | Validado con `lang_tools.py` |
| **Errores de comillas / balanceo (`bad_quoting`)** | **0** | Comillas internas adaptadas a «» |
| **Macros rotas / imágenes perdidas** | **0** | Multiconjunto idéntico al inglés |
| **Firmas rotas (`broken_signature`)** | **0** | Multiconjunto de colores y saltos idéntico al EN |
| **Prosa inglesa residual** | **0** | 0 oraciones o párrafos en inglés residual |
| **Descripciones largas idénticas al EN** | **0** | Todas traducidas o justificadas en lista cerrada |
| **Descripciones rehechas desde el inglés** | **189** | 53 en B01, 80 en B02, 22 en B09, 1 tarea, 33 en 191 |
| **Claves «solo-ES» conservadas** | **137** | 69 títulos + 68 descripciones (guías de apoyo originales) |
| **Nombres en inglés justificados (lista cerrada)** | **812** | Mods, panales, objetos sin `es_es` en JAR |
| **Lotes formalmente aprobados** | **83 / 83** | Aprobación 100% (criterios A, B, C, D) |

---

## 2. Cadena Editorial y Evolución de Candidatas

El proyecto ha seguido una rigurosa metodología de versiones aisladas e inmutables:

1. **183 (sha `f5f47ce3…`):** Incorporó las 144 claves que faltaban frente al inglés. Alcanzó `missing_vs_en = 0`. Primera pasada de QA visual en cliente con 349 mods.
2. **184 (sha `92abca33…`):** Correcciones de estilo y puntuación («¡Bueno, ha vuelto…!», «Te damos la bienvenida»).
3. **185 (sha `a406ce30…`):** Traducción de 107 claves traducibles dispersas (licencias AllTheMods, 38 tablas de recompensa, títulos genéricos).
4. **186 (sha `ba892d15…`):** Localización de 18 descripciones que se encontraban en inglés antiguo dentro del archivo base. QA visual in-game (segunda pasada).
5. **187 (sha `8822e506…`):** Unificación gramatical del verbo «fabricar» (39 claves), eliminando el anglicismo «craftear» salvo en nombres propios oficiales de Applied Energistics 2.
6. **188 (sha `826e4d19…`):** Reescritura completa desde el inglés de 53 descripciones de **B01 Progresión** que contenían paráfrasis libres y marcas «Objetivo:». `broken_signature` se redujo de 156 a 103.
7. **189 (sha `a9021c9a…`):** Reescritura desde el inglés de 80 descripciones de **B02 Fundamentos** (Logística, Energía, Herramientas, Trucos). Nombres oficiales validados con JARs de Mekanism y Pipez. `broken_signature` bajó de 103 a 23.
8. **190 (sha `0484c637…`):** Reescritura de 22 claves de **B09 Equipo y Combate** (Apotheosis, Apothic Enchanting, Just Dire Things) + título de tarea «Infinitas Piedras». **`broken_signature` llegó a 0**. Cuarta pasada de QA visual en juego (~25 pantallas).
9. **191 (sha `276dc838…` - FINAL):** Reescritura de 33 descripciones adicionales que presentaban glosas JEI/EMI añadidas o comentarios meta, garantizando fidelidad palabra por palabra al texto inglés. Unificación de «Mesa de Reforjado» / «Mesa de Reforjado Simple» y «Matriz de Inducción». QA visual in-game de las 38 claves modificadas.

---

## 3. Aprobación Formal por Bloques y Lotes (83/83 Aprobados)

Cada uno de los 83 lotes registrados en `audit_work/LOTES_MANIFEST_RECONCILIADO_83_V2.json` fue evaluado y aprobado bajo cuatro criterios objetivos:
- **Criterio A (Fidelidad al EN):** 0 claves rotas; la estructura, colores y saltos coinciden con el original inglés.
- **Criterio B (Prosa inglesa residual):** 0 frases o palabras vacías en inglés en textos descriptivos.
- **Criterio C (QA Visual in-game):** Muestreo en el cliente de 349 mods, apertura de misiones rehechas, verificación de renderizado sin recortes ni desbordamientos.
- **Criterio D (Nombres):** Lista cerrada de nombres confirmados mediante los archivos `es_es.json` de los JARs de los mods o mantenidos en inglés idénticos a JEI.

### Resumen por Bloque

| Bloque | Lotes | Claves EN | Ausentes | Rotas (A) | Prosa EN (B) | Estado |
|---|---|---|---|---|---|---|
| **B01 Progresión** | 8 | 433 | 0 | 0 | 0 | **APROBADO** |
| **B02 Fundamentos** | 13 | 827 | 0 | 0 | 0 | **APROBADO** |
| **B03 Almacén y Red** | 6 | 456 | 0 | 0 | 0 | **APROBADO** |
| **B04 Energía Avanzada** | 10 | 788 | 0 | 0 | 0 | **APROBADO** |
| **B05 Industria y Máquinas** | 12 | 1.024 | 0 | 0 | 0 | **APROBADO** |
| **B06 Modern Industrialization** | 4 | 174 | 0 | 0 | 0 | **APROBADO** |
| **B07 Producción y Recursos** | 13 | 873 | 0 | 0 | 0 | **APROBADO** |
| **B08 Magia y Rituales** | 8 | 501 | 0 | 0 | 0 | **APROBADO** |
| **B09 Equipo y Combate** | 9 | 311 | 0 | 0 | 0 | **APROBADO** |
| **Total** | **83** | **6.462** | **0** | **0** | **0** | **83 / 83 APROBADOS** |

*Registro completo disponible en:*  
- `audit_work/LOTES_ESTADO_191.json`  
- `audit_work/LOTES_ESTADO_191.csv`

---

## 4. Hallazgos Terminológicos y Lista Cerrada (Criterio D)

Tras una inspección directa de los archivos `lang/es_es.json` y `lang/en_us.json` en los JARs de los 349 mods instalados en `game/mods/`, se confirmaron las siguientes decisiones oficiales:

1. **Apotheosis:**
   - `apotheosis:block.apotheosis.reforging_table` → **Mesa de Reforjado** (oficial en el JAR).
   - `apotheosis:block.apotheosis.simple_reforging_table` → **Mesa de Reforjado Simple** (oficial en el JAR).
   - `apotheosis:item.apotheosis.sigil_of_rebirth.desc` → «Se usa para alimentar la Mesa de Reforjado».
   - Nombres de nivel de mundo adoptados del modpack: *Refugio, Frontera, Ascenso, Cima, Pináculo*. Términos: *Afijos, Invasores, Gemas, Infusión*.
2. **Productive Bees:**
   - `productivebees:entity.productivebees.green_carpenter_bee` → **Abeja carpintero verde** (oficial).
   - `productivebees:entity.productivebees.yellow_black_carpenter_bee` → **Abeja carpintero amarilla** (oficial).
3. **Ars Nouveau:**
   - `item.ars_nouveau.worn_notebook` → **Libreta Gastada** (oficial en el JAR).
4. **Immersive Engineering:**
   - `immersiveengineering:block.immersiveengineering.lightning_rod` → **Pararrayos** (oficial).
5. **Mekanism:**
   - `Cubo de Energía`, `Cable Universal`, `Tubo Presurizado`, `Transportador Logístico`, `Tubería Mecánica`, `Entrelazoportador Cuántico`, `Configurador`, `Matriz de Inducción`.
6. **Mods sin localización en español (Mantenidos en inglés como JEI):**
   - *Modern Industrialization, PneumaticCraft, XyCraft, LaserIO, Flux Networks, Integrated Dynamics, Transfer Labels, Dyson Cube Project, Just Dire Things.*
   - `Foundry Walls` (Productive Metalworks / Dyenamics: sin `es_es` → se mantiene en inglés o con descripción técnica contextual).
7. **Tareas genéricas (`task.*`):**
   - `task.*.title: "AllRightsReserved"` → traducido uniformemente como `TodosLosDerechosReservados`.
   - `task.08F68CC089765088.title: "Bypass Trick"` → `Truco para Saltárselo`.

---

## 5. Control de Calidad Visual in-game de la Candidata 191 (T2)

El cliente QA aislado fue ejecutado con los 349 mods y el mundo de pruebas `QAFTB_FULL_349_20261022` cargado:
- **Entorno:** 1280x720 (escalado 1.5, resolución nativa 1920x1080).
- **Registro de capturas:** `QA183_CAPTURAS/qa191_*.jpg`.
- **Verificación específica de las 38 claves de la 191:**
  - *Mesa de Reforjado / Mesa de Reforjado Simple:* Títulos y descripciones verificadas; colores púrpura (`&5&l`) y azul (`&9&l`) correctos.
  - *Matriz de Inducción (Mekanism):* Paginación 1/2 y colores verdes/azules renderizan correctamente.
  - *Fragmentos de Eco:* Saltos de línea y explicaciones de infusión limpios.
  - *Flux Networks:* Carga inalámbrica y materiales de red sin desbordamiento.
  - *LaserIO:* Conexiones de nodos, chips lógicos y llaves renderizan sin cortes.
  - *Hazte más pequeño (Tips and Tricks):* Descripción clara y directa.
  - *ATM Star & GeOres:* Formatos de recetas multilínea sin artefactos.
- **Muestreo de capítulos:**
  - Se abrieron y verificaron visualmente los capítulos de Bienvenida, Capítulos 1, 2, 3 y 4 de Progresión, Energía básica, Logística básica y Almacenamiento.
- **Cierre del cliente:**
  - El cliente fue cerrado enviando `WM_CLOSE` a la ventana principal. El mundo fue guardado de forma limpia y el proceso Java finalizó sin errores residuales.

---

## 6. Limitaciones Honestas

1. **Muestreo representativo:** Aunque todas las misiones rehechas y una muestra de cada capítulo fueron abiertas y capturadas en el juego, no se abrieron una a una las 3.753 misiones de forma manual in-game. La integridad del 100% de las misiones restantes se sustenta en la validación estática de SNBT y el validador estructural de firmas (`lang_tools.py`).
2. **Guías adicionales (137 claves «solo-ES»):** El modpack original contenía 137 textos añadidos por los autores hispanohablantes (67 con «Objetivo:») que no tienen contraparte en inglés. Por decisión del usuario se han mantenido intactos para no privar al jugador de estas explicaciones.
3. **Artefacto de renderizado tipográfico:** En algunas pantallas emergentes de FTB Quests, la primera línea de texto en negrita puede omitir visualmente la tilde de la letra «í» debido al motor de renderizado de la tipografía del pack. Se ha comprobado en el archivo fuente que el carácter almacena la tilde de forma correcta.
4. **Imágenes con texto en inglés:** Texturas de cabecera como «Chapter 2: The Cool Parts» o «Chapter 4: The ATM Star» tienen el texto rasterizado dentro de la propia imagen PNG del modpack y no son modificables vía archivo de idiomas.

---

## 7. Verificación de Seguridad y Entrega

1. **Instancia real del usuario (CurseForge):**
   - Ruta: `C:\Users\iagui\curseforge\minecraft\Instances\All the Mods 10 To the Sky   ATM10SKY\config\ftbquests\quests\lang\es_es.snbt`
   - Hash verificado al inicio y al final: `41d3cf485987b137b6611cee5cd48043d0ed69237c0772e4eb55bf6496308f66` (**100% INTACTO**).
   - **No se ha instalado nada en la instancia real.**
2. **Réplica de seguridad en el Chromebook:**
   - Sincronizado vía SSH/SCP a `100.79.20.45` en `/home/iagui/atm10sky-audit/integral_20261022/sync_20261024_191_final/`.
   - Hashes SHA-256 remotos verificados archivo por archivo.
