# Plantilla: documento in-world

> Para bitácoras, diarios, notas, cartas, libros/crónicas y escenas.
> Nombre de archivo: `AAAA-MM-DD_tipo_autor_titulo-corto.md` (ver `_convenciones.md`).

```markdown
---
idioma: es
formato: bitacora | diario | nota | carta | libro | cronica | escena
autor: …                      # personaje, institución o "anónimo"
destinatario: …               # solo cartas; si no aplica, "ninguno"
fecha_inworld: AAAA-MM-DD     # AAAA-00-00 si se desconoce
periodo: pre-5500 | invierno-5501 | presente
lugar: …                      # Por definir si no se sabe
estado_canon: BORRADOR | CANON
conocimiento_del_narrador: …  # qué sabe y qué no; sesgos
referencias: []               # eventos, personajes o archivos relacionados
---

# Título

(Texto del documento, en la voz del autor.)

---
**Notas de edición (fuera del mundo):**
- Fuente de los hechos: (jugador / partida / propuesta de Claude)
- Dependencias de canon: …
- Posibles incoherencias a revisar: …
```

## Guía rápida de voz por formato

| Formato | Encabezado típico | Registro | Cuidado con |
|---|---|---|---|
| Bitácora | Fecha + número de entrada | Institucional, conciso, hechos | No filtrar emociones personales; solo 5501+ |
| Diario / nota | Fecha o sin fecha | Íntimo, subjetivo | Que el autor no sepa más de lo que debe |
| Carta | Lugar, fecha, saludo, despedida | Epistolar | Fecha explícita; el remitente puede ser ajeno a la colonia |
| Libro / crónica | Título, autor, época | Académico, filosófico o histórico | Normalmente pre-5500 o de fuera |
| Escena | Contexto + diálogos | Literario, perspectiva meta | Marcar que es WIP y fuera de personaje |
