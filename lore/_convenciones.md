# Convenciones del repositorio

## 1. Estados de canon

Cada dato relevante (ficha, evento de la cronología, párrafo de facción…) puede llevar una etiqueta:

| Estado | Significado | Quién lo asigna |
|---|---|---|
| `CANON` | Aprobado por el jugador. Cambiarlo es un retcon. | Solo el jugador |
| `BORRADOR` | Escrito a partir de lo que el jugador ha contado, pendiente de revisión. | Claude o jugador |
| `PROPUESTA` | Idea sugerida por Claude. No es historia. | Claude |
| `OBSOLETO` | Sustituido por un retcon. Se conserva como referencia. | Tras un retcon aprobado |
| `Por definir` | Hueco sin información. **No se rellena inventando.** | — |

Formato en línea: `**[CANON]**`, `**[BORRADOR]**`, etc., al inicio del dato o de la sección.

## 2. Nombres de archivo y carpetas

- `snake_case`, en minúsculas, **sin tildes, eñes ni espacios** (compatibilidad entre sistemas y con la futura rama en inglés).
- Los archivos y carpetas de primer nivel llevan prefijo numérico de dos dígitos (`00_`…`10_`) para fijar el orden.
- Archivos de apoyo (no lore) empiezan por guion bajo: `_convenciones.md`, `_registro_retcons.md`, `_plantillas/`.

### Documentos in-world (dentro de `03_`, `04_`, `05_`, `10_`)

```
AAAA-MM-DD_tipo_autor_titulo-corto.md
```

- `AAAA-MM-DD`: fecha **in-world** (año, mes, día del calendario de la colonia; ver `00_cronologia.md`). Si solo se conoce el año o el mes, usa `AAAA-MM-00` o `AAAA-00-00`. Si es anterior al 5500 y la fecha exacta se ignora, `AAAA-00-00`.
- `tipo`: `bitacora`, `diario`, `nota`, `carta`, `libro`, `cronica`, `escena`.
- `autor`: nombre en minúsculas sin tildes (`kliff`, `unkas`, `ina`, `tarylla`, `zorro`, `zhethe`, `yuld`…) o `anonimo` / `institucional`.
- `titulo-corto`: 2–5 palabras con guiones.

Ejemplos (solo ilustran el formato; no son documentos reales):
`5501-03-12_bitacora_institucional_primera-nevada.md`
`5501-04-02_carta_anonimo_aviso-del-norte.md`

Una **obra larga** (libro, crónica) puede ser una carpeta con el mismo patrón y un `indice.md` dentro.

### Fichas de personaje
Se mantienen todas en `01_personajes.md` mientras sean breves. Cuando una ficha crezca, pasa a `01_personajes/nombre.md` (nombre en minúsculas, sin tildes) y `01_personajes.md` queda como índice. Usa `_plantillas/ficha_personaje.md`.

## 3. Fechas y calendario

- El año de la historia se escribe con cuatro cifras: **5500**, **5501**.
- Tres grandes periodos: **Pre-5500** · **Invierno del 5501** · **Presente / registro oficial posterior**.
- El calendario exacto de la colonia (meses, estaciones, equivalencias con RimWorld) está **por definir**; anótalo en `00_cronologia.md` cuando el jugador lo fije.
- Distingue siempre **fecha in-world** de **fecha de la partida/real**; no las mezcles en el mismo campo.

## 4. Enlaces y referencias

- Enlaces relativos entre archivos: `[Kliff](../01_personajes.md#kliff)`.
- Un personaje se menciona por su nombre tal cual figura en la ficha.
- Toda ficha de facción, lugar o criatura es la fuente de verdad; en los demás archivos se resume y se enlaza.

## 5. Trazabilidad de fuentes (para el modo `Canon-Only`)

Al final de cada documento in-world, incluye la cabecera completa de la plantilla (autor, destinatario, fecha, formato, nivel de conocimiento del narrador, estado de canon). Así un lector externo, humano o IA, puede evaluar la fiabilidad del texto sin contexto añadido.

## 6. Preparación para una rama en inglés

La versión canónica es la española. Para una futura traducción:

- Se recomienda una **rama `en`** (o carpeta `lore_en/`) que **conserve exactamente los mismos nombres de archivo** que `lore/`, de modo que los enlaces y el mapa sigan valiendo.
- Cada archivo lleva una cabecera con `idioma: es`. En la rama en inglés se cambia a `idioma: en` y se añade `traduccion_de: <commit o fecha>`.
- Los nombres propios (Kliff, Unkas, El Umbral, GAPA…) se mantienen; los de facciones y lugares con traducción se anotan en un glosario `_glosario_es_en.md` (a crear cuando empiece la traducción).
- Los retcons y el canon se deciden en español; la rama inglesa los sigue, no los adelanta.

## 7. Commits y ramas

- Mensajes de commit en español, en imperativo corto: `Añade ficha de Zorro`, `Retcon: nuevo origen de El Umbral`.
- Los cambios sobre canon aprobados se mencionan en el commit y en `_registro_retcons.md`.
- `Library/` nunca forma parte de commits de Claude salvo petición explícita del jugador.
