<div align="center">

# 🌌 All The Mods 10: To The Sky
### 🇪🇸 Traducción al español (`es_es`) del libro de misiones FTB Quests

[![Minecraft](https://img.shields.io/badge/Minecraft-1.21.1-2EA44F?style=for-the-badge&logo=minecraft&logoColor=white)](https://www.minecraft.net/)
[![NeoForge](https://img.shields.io/badge/NeoForge-1.21.1-E06C75?style=for-the-badge)](https://neoforged.net/)
[![Pack](https://img.shields.io/badge/ATM10%20To%20the%20Sky-v2.0.7-61AFEF?style=for-the-badge)](https://www.curseforge.com/minecraft/modpacks/all-the-mods-10-sky)
[![Claves](https://img.shields.io/badge/Claves%20ausentes%20vs%20EN-0%20de%206.462-98C379?style=for-the-badge)](AUDIT_REPORT.md)
[![Estado](https://img.shields.io/badge/Estado-candidata%20191%20%C2%B7%20revisi%C3%B3n%20est%C3%A1tica%20%2B%20muestreo-56B6C2?style=for-the-badge)](AUDIT_REPORT.md)

<p align="center">
  <b>Traducción al español de España de las misiones de ATM10: To the Sky v2.0.7, con revisión estática completa y muestreo en el juego.</b><br>
  <i>Cobertura del 100 % de las claves del inglés · colores, saltos de línea e imágenes conservados · nombres alineados con los JAR de los mods cuando existen.</i>
</p>

[📖 Resumen](#-resumen) •
[✅ Qué está verificado](#-qué-está-verificado-y-qué-no) •
[🎮 Capturas](#-capturas-del-cliente) •
[📥 Cómo instalar](#-cómo-instalar-y-jugar) •
[📄 Informe técnico](AUDIT_REPORT.md)

---

</div>

## 📖 Resumen

Este repositorio contiene `es_es.snbt`, el archivo de idioma de FTB Quests para **All The Mods 10: To the Sky v2.0.7** (Minecraft 1.21.1, NeoForge, 349 mods), en español de España.

- **Cobertura:** las **6.462 claves** de `en_us.snbt` tienen su equivalente en `es_es.snbt` (0 ausentes).
- **Formato intacto:** se comprobó con validadores propios que no hay errores de parseo SNBT, de comillas, de macros ni de imágenes, y que cada texto conserva el mismo multiconjunto de códigos de color y saltos de línea que el inglés (`broken_signature = 0`).
- **189 descripciones rehechas desde el inglés:** eran paráfrasis libres, con marcas «Objetivo:» o glosas añadidas; se reescribieron siguiendo el texto fuente (156 en la tanda B01/B02/B09 y 33 en la candidata 191).
- **137 guías «solo en español» conservadas:** son textos de los autores originales del pack (69 títulos y 68 descripciones) que **no existen en el inglés**. Se dejaron tal cual por decisión del autor de la traducción, porque explican cosas útiles del inicio de la isla. Por eso no son una traducción literal del inglés.
- **Nombres:** cuando el JAR de un mod trae `es_es.json` con un nombre distinto, se usa el oficial; si no, se deja el inglés tal como aparece en JEI. No se inventan nombres.
- **Terminología:** «craftear» se unificó a «fabricar», salvo nombres propios oficiales.

> [!IMPORTANT]
> Esta traducción es un trabajo comunitario y no está afiliada a All The Mods. No ha sido revisada ni aprobada por el equipo de ATM.

---

## ✅ Qué está verificado y qué no

| Comprobación | Resultado | Cómo se comprobó |
|---|:---:|---|
| Claves ausentes frente a `en_us.snbt` | **0 de 6.462** | Comparación automática de claves |
| Errores de parseo SNBT / comillas / macros / imágenes | **0** | Validador propio |
| Firmas de color y saltos de línea rotos (`broken_signature`) | **0** | Validador propio |
| Descripciones rehechas desde el inglés | **189** | Registro de reescrituras por candidata |
| Guías «solo-ES» conservadas | **137** | Comparación de claves con el inglés |
| Muestreo en el juego de la candidata 190 | ~25 pantallas, **sin errores de FTB Quests** | Cliente de prueba con los 349 mods |
| Las 38 claves cambiadas en la candidata 191 | **No se comprobaron una a una en el juego** | Solo validación estática |
| Revisión visual de las 3.753 misiones una a una | **No realizada** | Se hizo muestreo, no revisión completa |

Lo que **no** se afirma:

- No hay aprobación visual en el juego «por lotes». Los 83 lotes de `LOTES_ESTADO_191.*` son un registro interno de trabajo (criterios estáticos) y **no** equivalen a 83 revisiones visuales independientes; además, los totales por bloque de esos ficheros no suman 6.462 y no deben usarse como cifra oficial.
- La prosa en inglés residual se buscó con un detector heurístico; no es una garantía formal de que no quede ningún texto en inglés.
- No se ha probado un flujo automatizado de traducción para otros modpacks.

Detalles y limitaciones en [`AUDIT_REPORT.md`](AUDIT_REPORT.md).

> [!NOTE]
> **Huella del archivo** (SHA-256 de `es_es.snbt`, candidata 191):  
> `276dc8389226097fc726d77a5d9412f339277518ec23417a6eefa48044868209`  
> Si clonas el repositorio en Windows con `core.autocrlf=true`, Git puede cambiar los finales de línea y el hash local será distinto; el contenido almacenado en el repositorio sí coincide con esta huella.

---

## 🎮 Capturas del cliente

Son capturas **reales** del cliente de Minecraft con ATM10: To the Sky v2.0.7 y los 349 mods, tomadas durante las sesiones de prueba de las candidatas 183 a 190. **No se regeneraron con la candidata 191**, así que algunos textos pueden diferir ligeramente del archivo final. Sirven para ver el aspecto general, no como prueba de cada clave.

### Menú y vista general
<table width="100%">
  <tr>
    <td width="50%" align="center">
      <b>Menú principal del pack</b><br>
      <img src="screenshots/mc_01_main_menu.jpg" alt="Menú principal de ATM10" />
    </td>
    <td width="50%" align="center">
      <b>Vista general de capítulos</b><br>
      <img src="screenshots/mc_02_quests_overview.jpg" alt="Vista general de FTB Quests" />
    </td>
  </tr>
</table>

### Inicio del pack
<table width="100%">
  <tr>
    <td width="50%" align="center">
      <b>Misión de bienvenida</b><br>
      <img src="screenshots/mc_03_welcome_quest.jpg" alt="Misión de bienvenida" />
    </td>
    <td width="50%" align="center">
      <b>Capítulo 1: primeros pasos</b><br>
      <img src="screenshots/mc_04_chapter1_starting_out.jpg" alt="Capítulo 1" />
    </td>
  </tr>
</table>

### Capítulos de mods y ventanas de misión
<table width="100%">
  <tr>
    <td width="50%" align="center">
      <b>Capítulo de Mekanism</b><br>
      <img src="screenshots/mc_05_mekanism_chapter.jpg" alt="Capítulo de Mekanism" />
    </td>
    <td width="50%" align="center">
      <b>Mekanism: ventana «Máquinas»</b><br>
      <img src="screenshots/mc_06_mekanism_popup.jpg" alt="Ventana de misión de Mekanism" />
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <b>Capítulo de Create</b><br>
      <img src="screenshots/mc_10_create_chapter.jpg" alt="Capítulo de Create" />
    </td>
    <td width="50%" align="center">
      <b>Ars Nouveau: Mesa de Escriba</b><br>
      <i>Texto largo con desplazamiento vertical</i><br>
      <img src="screenshots/mc_09_ars_nouveau_popup.jpg" alt="Ventana de Ars Nouveau" />
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <b>HNN: página 1</b><br>
      <img src="screenshots/mc_07_hnn_datacenter.jpg" alt="HNN página 1" />
    </td>
    <td width="50%" align="center">
      <b>HNN: página 2 con imagen incrustada</b><br>
      <img src="screenshots/mc_08_hnn_page2_image.jpg" alt="HNN página 2" />
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <b>Consejos de construcción</b><br>
      <img src="screenshots/mc_11_building_tips_popup.jpg" alt="Consejos de construcción" />
    </td>
    <td width="50%" align="center">
      <b>Functional Storage</b><br>
      <img src="screenshots/mc_12_storage_popup.jpg" alt="Functional Storage" />
    </td>
  </tr>
</table>

---

## 📥 Cómo instalar y jugar

1. Descarga [`es_es.snbt`](es_es.snbt) de este repositorio.
2. Cierra Minecraft y CurseForge.
3. **Haz una copia de seguridad.** Ve a la carpeta de tu instancia:  
   `curseforge\minecraft\Instances\All the Mods 10 To the Sky   ATM10SKY\config\ftbquests\quests\lang\`  
   y copia tu `es_es.snbt` actual con otro nombre (por ejemplo `es_es.snbt.backup`).
4. Pega el `es_es.snbt` descargado en esa carpeta, reemplazando el anterior.
5. Abre el juego y elige **Español (España)** en *Opciones → Idioma*.

Para volver atrás, restaura la copia de seguridad.

> [!TIP]
> Descarga el archivo con el botón «Raw» o «Download raw file». Si lo copias a mano, asegúrate de guardarlo como UTF-8.

---

## 📂 Contenido del repositorio

```text
├── es_es.snbt                 # Archivo de idioma (candidata 191)
├── README.md                  # Este documento
├── AUDIT_REPORT.md            # Informe técnico: qué se comprobó, cómo y con qué límites
├── LOTES_ESTADO_191.json      # Registro interno de lotes de trabajo (no es una aprobación visual; totales no fiables)
├── LOTES_ESTADO_191.csv       # Lo mismo, en CSV
└── screenshots/               # Capturas reales del cliente de pruebas (candidatas 183–190)
```

---

<div align="center">
  <sub>Traducción y revisión por <b>Iago Roibas</b> (@iagorobo24-hub), con asistencia de IA para redacción y validación.</sub><br>
  <sub><i>All The Mods y FTB Quests son marcas de sus respectivos creadores. Proyecto comunitario sin ánimo de lucro.</i></sub>
</div>
