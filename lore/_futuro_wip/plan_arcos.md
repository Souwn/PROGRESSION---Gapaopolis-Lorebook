---
idioma: es
formato: plan
autor: Claude (propuesta para el jugador)
fecha_inworld: Por definir (futuro)
periodo: futuro
estado_canon: PROPUESTA
---

# Plan de los arcos 3 a 6 (dirección prevista)

> **Esto no es canon ni historia ocurrida.** Es una propuesta de método y de orden de eventos, hecha a partir de las listas del jugador, de lo ya archivado y de la carpeta `_futuro_wip/`. Todo lo que aparece aquí es `PROPUESTA` salvo que se indique lo contrario, y nada pasa a canon sin la aprobación explícita del jugador (regla de oro de [`CLAUDE.md`](../CLAUDE.md) §4.1).
> **Modo `Canon-Only`: este archivo no cuenta.** Contiene información de autor (`META`) y hechos aún no ocurridos; solo se usa en `Interactive`. Nada de lo que hay aquí puede filtrarse a un texto in-world que el personaje no podría conocer.
> Los enlaces a `planes_futuros.md` y a `zorro_visita-de-emisarios.md` funcionan cuando se fusione el PR #8, que crea esta carpeta.

## Índice

1. [Método](#1-método)
2. [Punto de partida: lo que ya hay](#2-punto-de-partida-lo-que-ya-hay)
3. [Arco 3 · «Problemas en casa»](#3-arco-3--problemas-en-casa)
4. [Arcos 4 a 6 (esquema)](#4-arcos-4-a-6-esquema)
5. [Incoherencias y tensiones detectadas](#5-incoherencias-y-tensiones-detectadas)
6. [Preguntas que necesito del jugador](#6-preguntas-que-necesito-del-jugador)

---

## 1. Método

### 1.1 Jerarquía

| Nivel | Qué es | Ejemplo |
|---|---|---|
| **Arco** | Un tramo de la historia con un tema y un cierre propios. | Arco 3 · «Problemas en casa» |
| **Hilo** | Una línea de trama dentro del arco, con su propio principio, nudo y punto de llegada. | Hilo A · Sospechas y conspiraciones |
| **Evento** | Algo que cambia de verdad el estado de un hilo. Es la unidad que se planifica. | A2 · Unkas descubre que la vigilan |
| **Texto** | La entrada in-world que cuenta el evento (diario, nota, carta, bitácora, escena). | Diario de Kliff, 8º de Junligosto |

Regla de oro del método: **se planifican eventos, no textos.** Un evento puede acabar en un texto, en varios o en ninguno. Si un evento no cambia nada, no es un evento.

### 1.2 Ficha de evento

Cada evento de este plan se describe con los mismos campos, para que cualquiera (persona o IA) pueda leerlo en segundos:

| Campo | Qué dice |
|---|---|
| **ID** | Letra del hilo + número (`A2`). No cambia aunque se reordene. |
| **Evento** | Una frase: qué pasa. |
| **Tipo** | `ANCLA` (ocurre sí o sí y su orden importa) · `FLEXIBLE` (ocurre dentro del arco, momento libre) · `RESERVA` (solo si el juego lo ofrece o lo permite). |
| **Depende de** | Eventos que deben haber ocurrido antes. |
| **Quién lo sabe** | Quién lo vive y quién lo ignora. Es lo más importante para evitar anacronismos de conocimiento. |
| **Texto previsto** | Formato y narrador sugeridos. |
| **Estado** | Ver 1.3. |

### 1.3 Estados de un evento

`IDEA` → `PLANEADO` (el jugador lo ha aprobado como dirección) → `EN PARTIDA` (el juego ya lo ha producido) → `ESCRITO` (hay un texto en borrador) → `CANON` (el jugador aprueba el texto) · también `APLAZADO` (no tocar todavía) y `DESCARTADO`.

Todos los eventos de este documento nacen como `IDEA`. Solo el jugador los sube de nivel.

### 1.4 Ritmo (acordado)

- **1 año de historia ≈ 3 años de juego.** Consecuencia práctica: el juego va varias veces más rápido que la historia. No todo lo que ocurre en la partida entra; el plan es el filtro. El calendario in-world (Marzimayo… Difebrero) lo asigna el plan, no se copia de la fecha de la partida.
- **Una entrada por personaje solo cuando algo cambia de verdad.** El número de textos es un techo, no una cuota. Un año tranquilo puede tener menos textos que uno agitado.
- **Una bitácora anual de resumen** (formato 1, institucional) que cierra cada año de historia. Contrasta a propósito con las notas privadas: la bitácora dice lo que la colonia está dispuesta a dejar por escrito; las notas, lo que de verdad pasó. Esa distancia es una fuente de tensión del arco 3.

### 1.5 Ciclo de trabajo por sesión de juego

1. El jugador manda el reporte en bruto → se anota en [`_diario_de_partida.md`](../_diario_de_partida.md).
2. Se contrasta con este plan: ¿qué evento ha producido el juego? ¿cuál se ha adelantado o retrasado? ¿qué ha sido emergente?
3. Se marca cada evento nuevo: `Adaptar ahora` · `Aplazar` · `Descartar` · `Hace falta un hilo nuevo`.
4. Se propone el texto (en el chat, no en el repositorio) y, si el jugador lo aprueba, se archiva.
5. Se actualiza el tablero del hilo (columna **Estado**) y se anotan las dudas nuevas en [`_preguntas_abiertas.md`](../_preguntas_abiertas.md).

### 1.6 Semáforo juego ↔ historia

El juego ya ha adelantado cosas que la historia no debe contar aún (pareja Kliff–Zorro, dos embarazos). El plan marca esos casos como `ADELANTADO EN PARTIDA`: existen en el juego pero siguen `APLAZADO` en el texto hasta que el jugador diga lo contrario. Ver [5.3](#53-el-juego-va-por-delante-de-la-historia).

### 1.7 Cuándo dividir este archivo

Mientras sea un solo documento, se lee mejor. Si el jugador lo aprueba, cada arco pasaría a su propio archivo (`arco_3.md`, `arco_4.md`…) con el mismo formato, y este quedaría como índice.

---

## 2. Punto de partida: lo que ya hay

Resumen de lo establecido a fecha de este plan (Marzimayo del 5502). Lo marcado `META` o `FUTURO` no es conocible por los personajes.

| Tema | Qué hay | Fuente |
|---|---|---|
| Kliff | Cumplido el segundo invierno «sin una sola desgracia» (según él). Quiere vigilar a Unkas y Zhethe, pero no sabe en quién confiar. `META`: paranoia que intentará ocultar; técnicamente inmortal y con psycasts sin saberlo. | [Diario de Kliff 2](../04_personales/), [`_meta_autor.md`](../_meta_autor.md) |
| Unkas | Escribió que Kliff le preocupa de verdad y que la gente lo evita. `META`: no planea marcharse, planea quedarse; lo que trama está por definir. Es una Exiliada que huyó de las montañas tomadas por los Ixthar. | Unkas II, `_meta_autor.md`, fichas |
| Zhethe | Dijo a Kliff «cosas imposibles» (un zombi con la apariencia de Liry). `No miente`. Tiene su propia choza junto a la puerta. | Diario de Kliff 5501, Zorro #5 |
| Tarylla | Perdió al mímico durante el invierno y lo ha descubierto ahora. Busca un sustituto de su estudio nocturno; la excusa son las camas. `META`: tres identidades (imperial, corrompida, leal), sin memoria de su pasado; la caja que enfría funciona con polvo de huesos del esqueleto sombrío. | Tarylla #6 (borrador), `_meta_autor.md` |
| Zorro | Vive en un barracón compartido; muralla nueva; ligero *crush* hacia Kliff; teme que la devuelvan al huerto. `META`: será la primera en enfrentarse a Kliff. | Relato de Zorro #5 |
| Yuld | Se fue el 1º de Septumbre del 5501 al rancho del este; su carta se perdió. `META`: no se reincorpora como pawn, pero volverá a aparecer. `META`: alguien encontró la carta y se deshizo de ella. | Carta de Yuld, `_meta_autor.md` |
| Tumbas | Las de Kaelen, Liry y Ozan aparecieron saqueadas y vacías el 15º de Difebrero del 5501. **Sin explicación.** | Diario de Kliff 5501 |
| Lexington / Krosswynd | Un minero (raza no humana) y un granjero (humano) llegados al juego. Sin lore. | [`_diario_de_partida.md`](../_diario_de_partida.md) |
| Obras | Muralla grande terminada; planes de templo, casas y túneles (lista del jugador). | Zorro #5, mensaje del jugador |
| `FUTURO` | Yuld vuelve en primavera con un relato de bárbaros que asaltan un carruaje y matan a su enviado (inicio de las guerras); Krosswynd se une. Visita de emisarios de las tres naciones (90 % segura). Guerra final perdida, rescate imperial, Kliff nombrado Terrateniente. | [`planes_futuros.md`](planes_futuros.md), [`zorro_visita-de-emisarios.md`](zorro_visita-de-emisarios.md) |

---

## 3. Arco 3 · «Problemas en casa»

### 3.1 Objetivo narrativo

> **Propuesta de tema:** la amenaza ya no viene de fuera, viene de dentro. Cada habitante guarda un secreto que, por separado, es defendible; juntos se vuelven una colonia en la que nadie confía en nadie. Coincide con lo que dijo el jugador: «la mayor amenaza para la colonia es la propia colonia».

Qué debe haber cambiado al cerrar el arco (propuesto):

1. Kliff, Unkas y Zorro han chocado de verdad, aunque ninguno ha ganado.
2. Tarylla ha cruzado un primer umbral (la nigromancia deja de ser teoría) y sabe algo más de sí misma, sin resolverlo.
3. Kliff ha vuelto de su viaje con un poder que la colonia no puede ignorar.
4. La colonia ha crecido físicamente: casas, templo, túneles.
5. Quedan abiertos los ganchos hacia el arco 4: el mundo exterior se acerca (Yuld, bárbaros, emisarios).

### 3.2 Mapa de dependencias

```
                      ┌──────────────────────────┐
                      │ F · Viaje de Kliff       │ ← pieza central
                      └────┬─────────┬───────┬───┘
         ausencia de Kliff │         │       │ vuelve con poder
                           ▼         ▼       ▼
        A · Sospechas ◄──► B · Tarylla    G · Kliff + Zorro
              ▲               │  ▲              ▲
              │               │  └─ C · Investigaciones (la caja que enfría)
              │               ▼
    D · Yuld / Zhethe     Tumbas, mímico, nigromancia
              │
              ▼
    E · Obras (casas, templo, túneles) ──► arco 4: Ixthar
```

Relaciones que sostienen el arco (todas `IDEA`):

| # | Relación | Por qué importa |
|---|---|---|
| 1 | **F → A, B, E:** mientras Kliff está fuera, Unkas dirige la colonia. | Convierte las sospechas de Kliff en algo que parece confirmarse al volver. |
| 2 | **F → G:** Zorro es la única que conoce la electricidad como concepto. | Un vínculo que nace de entender a Kliff, no solo de gustarle. |
| 3 | **F → B:** Tarylla es una espía imperial sin memoria; ve los poderes de Kliff. | Es la primera prueba real de cuál de sus tres identidades manda. |
| 4 | **B ↔ C:** la caja que enfría funciona con polvo de huesos; Zorro no sabe por qué. | Si Zorro intenta reproducirla y falla, descubre el secreto de Tarylla. |
| 5 | **Tumbas → A y B:** nadie sabe qué pasó. Kliff lo ignora; Zhethe vio un zombi. | Es el misterio central del arco y conecta paranoia con nigromancia. |
| 6 | **D → A:** Zhethe cuida a los animales; Yuld es su vínculo exterior. | Kliff puede sospechar que Zhethe y Yuld se entienden a sus espaldas. |
| 7 | **E → arco 4:** los túneles se acercan a la colonia de los Ixthar. | Siembra las guerras sin necesidad de un evento exterior. |

### 3.3 Hilos y eventos

#### Hilo 0 · «sin ideas» — el gancho de apertura

El jugador dejó este punto vacío. Lo trato como la **pieza que falta** para abrir el arco, no como un hilo más. Opciones propuestas (se elige una; las otras se descartan o se reciclan):

| Opción | Qué sería | A favor | En contra |
|---|---|---|---|
| **0a. El regreso de Yuld con malas noticias** (recomendada) | Yuld vuelve en primavera: el ganado está bien, pero su enviado murió asaltado por bárbaros. | Ya está en `FUTURO`; une «Yuld y animales» con el mundo exterior y con Zhethe. | Adelanta una amenaza externa en un arco «de casa». |
| 0b. El ataque del Ferroespanto | Reutiliza el ataque pendiente en el diario de partida y hace de él el detonante: Kliff manda vigilar al resto mientras se defienden. | Aprovecha un evento ya ocurrido en el juego. | Puede quedar «de relleno» si no cambia nada después. |
| 0c. La noche del mímico | El mímico reaparece (imitando algo o a alguien) y destapa que Tarylla sabía de él. | Pone la paranoia de Kliff delante de una amenaza literal («alguien no es quien dice ser»). | Adelanta la revelación de Tarylla. |

#### Hilo A · Sospechas y conspiraciones (Kliff vs. Unkas)

**Ya establecido:** Kliff vigila; Unkas teme por él; Zhethe «no es cómodo con él»; Zorro vio a Unkas y Zhethe besándose en el Templo; Kliff cree que conspiran juntos.
**Ironía dramática disponible (si se quiere usar):** Kliff ve una conspiración política donde quizá hay una relación sentimental (el embarazo de Unkas y Zhethe está `APLAZADO`, ver 5.3). Pero `META` dice que Unkas planea *algo* para quedarse: la sospecha de Kliff puede ser falsa en el motivo y cierta en el fondo.
**Hallazgo del lector:** Kliff concluye que fue Unkas quien habló a Zhethe de «cosas imposibles», pero Zhethe describe lo que vio él mismo (el zombi). Kliff se equivoca de culpable. Merece dejarse así.

| ID | Evento | Tipo | Depende de | Quién lo sabe | Texto previsto |
|---|---|---|---|---|---|
| A1 | Kliff empieza a vigilar de forma activa. Duda a quién pedir ayuda; una opción es elegir a un recién llegado (Lexington o Krosswynd) precisamente porque no tiene historia en la colonia. | FLEXIBLE | — | Solo Kliff (y el recién llegado) | Diario de Kliff |
| A2 | Unkas se da cuenta de que la vigilan y decide no confrontarlo todavía. | ANCLA | A1 | Unkas | Nota de Unkas (breve) |
| A3 | Zorro se enfrenta a Kliff por primera vez (`META`: será la primera en hacerlo). | ANCLA | A1 (o G1) | Zorro, Kliff; testigos por definir | Relato de Zorro |
| A4 | Unkas pone en marcha su plan (ver decisión **Q3**): un contrapeso, no una rebelión. | ANCLA | A2 | Unkas y quien ella elija | Nota de Unkas |
| A5 | Kliff toma una medida que no puede retirar (castigo, prohibición, destierro o encierro). Es el punto de no retorno del hilo. | ANCLA | A3, A4 | Colonia entera | Diario de Kliff + bitácora |
| A6 | Al volver del viaje (F), Kliff encuentra el poder de Unkas mayor del que esperaba, o ella el de Kliff. El hilo queda **abierto**, no resuelto. | ANCLA | F3, A4 | Todos | Bitácora anual |

**Huecos del hilo:** qué trama Unkas exactamente (Q3); si Kliff llega a actuar contra alguien (A5); cuándo se resuelve el hilo (propongo: arco 4, cuando la vuelta de Unkas con los Ixthar la expone).

#### Hilo B · Los delirios de Tarylla (dudas, decisiones y la puerta a la nigromancia)

**Ya establecido:** tres identidades (imperial, corrompida, leal); trauma del invierno; no recuerda su pasado; estudia anomalías a escondidas; lamenta haber perdido al mímico; Kliff la ve como una «friki indecente», sin sospechas claras.
**Qué significa «abrir la puerta a la nigromancia»** (propuesta de lectura, para confirmar): no que Tarylla resucite a alguien en el arco 3, sino que **da el primer paso deliberado** y el lector ve que habrá un segundo. La tentación más natural en la historia son los tres cuerpos desaparecidos.

| ID | Evento | Tipo | Depende de | Quién lo sabe | Texto previsto |
|---|---|---|---|---|---|
| B1 | La búsqueda del mímico (ya iniciada en Tarylla #6): revisa camas, taburetes y paredes. Su excusa son los muebles. | ANCLA | — | Solo Tarylla | Tarylla #6 y siguientes |
| B2 | Resultado de B1 (ver decisión **Q5**): lo encuentra, no lo encuentra, o *él* la encuentra a ella. | ANCLA | B1 | Tarylla (y quien lo vea) | Nota de Tarylla |
| B3 | Primer destello de memoria: un objeto, un olor o un nombre le recuerda su vida imperial. No resuelve nada, solo la asusta. | FLEXIBLE | — | Solo Tarylla | Nota de Tarylla |
| B4 | Descubre o sospecha algo sobre las tumbas vacías: sabe más que nadie sobre lo que puede levantar a un cuerpo. | ANCLA | Tumbas, B2 | Solo Tarylla | Nota de Tarylla |
| B5 | **La decisión:** dejar de investigar «a medias» y probar algo con un muerto, con el polvo de huesos o con el esqueleto cautivo. Ver **Q6**. | ANCLA | B4 | Solo Tarylla | Nota de Tarylla |
| B6 | Ve los poderes de Kliff (F3). Tiene que decidir si se lo calla, y por qué. | ANCLA | F3 | Tarylla, Kliff | Nota de Tarylla |

**Huecos del hilo:** quién profanó las tumbas (**Q4**); si la tentación es personal (Kaelen, Liry u Ozan) o científica; cuánto ve el lector de B5 (se puede mostrar solo el «después»).
**Hipótesis, no propuesta cerrada:** la «Tarylla corrompida» podría haber estado detrás de las tumbas sin saberlo. Encaja con su pérdida de cabeza y con sus tres identidades. Solo se usa si el jugador lo aprueba.

#### Hilo C · Investigaciones

**Ya establecido:** Zorro y Tarylla colaboran desde el final del otoño del 5501; la caja que enfría funciona gracias al polvo de huesos (`META`); Tarylla afirma que son «hongos mágicos con sal». Descubiertos en partida: pemmican, camas nuevas, retretes, «etc.»; pendiente de volcar en [`09_tecnologia.md`](../09_tecnologia.md).
**Método propuesto para investigar sin inventar:** cada hito del árbol de investigación del juego se convierte en un *mini-evento* con tres campos, y solo entra en el lore si cumple al menos uno:
1. **¿Cambia la vida de la colonia?** (comida, salud, defensa).
2. **¿Revela o esconde algo?** (Zorro decide qué calla; Tarylla oculta su método).
3. **¿Genera conflicto?** (alguien no lo entiende, alguien se opone, alguien lo teme).

| ID | Evento | Tipo | Depende de | Quién lo sabe | Texto previsto |
|---|---|---|---|---|---|
| C1 | Higiene y confort: retretes y camas de paja (primeras mejoras visibles). | RESERVA | Partida | Toda la colonia | Bitácora |
| C2 | Zorro intenta reproducir la caja que enfría y no lo consigue. | FLEXIBLE | — | Zorro | Relato de Zorro |
| C3 | Zorro sospecha que Tarylla le oculta un ingrediente. No lo dice. | ANCLA | C2 | Zorro | Relato de Zorro |
| C4 | Tarylla tiene que contarle algo a Zorro (verdad parcial) o dejar que se aparte. Es la primera vez que dos secretos chocan entre colonos. | ANCLA | C3 | Zorro, Tarylla | Nota o escena |
| C5 | Un avance nuevo (a decidir según lo que el juego dé) que Zorro entiende de una civilización mucho más avanzada y que decide frenar o disfrazar. | RESERVA | Partida | Zorro | Relato de Zorro |

**Huecos del hilo:** la tabla «Conocimientos de Zorro» de [`09_tecnologia.md`](../09_tecnologia.md) sigue vacía. Antes de C5 hay que decidir qué sabe y qué calla.

#### Hilo D · Yuld y los animales

**Ya establecido:** Yuld se marchó a un rancho del este, defiende su sitio con flechas, `META`: volverá a aparecer sin reincorporarse. `FUTURO`: vuelve en primavera con un relato de bárbaros que asaltan un carruaje y matan a su enviado. Zhethe es ahora el cuidador principal.
**Sorpresa útil:** `META` dice que alguien encontró la carta de Yuld y se deshizo de ella. Si Yuld vuelve en persona, la carta se vuelve irrelevante para Kliff pero no para quien la destruyó.

| ID | Evento | Tipo | Depende de | Quién lo sabe | Texto previsto |
|---|---|---|---|---|---|
| D1 | Yuld regresa a Gapaopolis en primavera y explica su situación. | ANCLA | — | Colonia entera | Escena o diario |
| D2 | El relato de los bárbaros: carruaje asaltado, enviado muerto. Es la chispa de «las guerras». | ANCLA | D1 | Yuld, Kliff, Zhethe | Diario de Kliff |
| D3 | Reacción de Kliff: ¿perdón, rencor o frialdad? Después de «traición» (así lo vivió), ahora le debe algo. | ANCLA | D1 | Kliff, Yuld | Diario de Kliff |
| D4 | Intercambio de ganado entre colonia y rancho; Zhethe y Yuld hablan a solas. | FLEXIBLE | D1 | Zhethe, Yuld | Nota de Zhethe (primera voz suya) |
| D5 | Yuld se marcha otra vez (o se queda un tiempo breve). `META`: no vuelve a ser pawn. | ANCLA | D2 | Todos | Bitácora |
| D6 | Krosswynd se une (`FUTURO`: «para ayudar»). | ANCLA | D2 | Todos | Bitácora |

**Huecos del hilo:** si Kliff sospecha de Zhethe y Yuld juntos (extiende A); quién fue el enviado muerto (¿un personaje nuevo?); qué es el «carruaje» en un mundo de transición animal-neolítica (puede ser carro de tiro; ver 5.6).

#### Hilo E · El nuevo templo, las nuevas casas y los túneles

**Ya establecido:** el templo actual es una sala en cruz sobre el almacén, dentro de la montaña. Zorro vive en un barracón compartido; Zhethe tiene choza propia. Lexington es minero; Ina es constructora y minera. Los túneles no están descritos.
**Idea de fondo:** cada obra es también una decisión política. Quién recibe casa propia, quién queda en el barracón, hacia dónde cavan los túneles y para qué sirve el templo nuevo dicen más de la colonia que cualquier discurso.

| ID | Evento | Tipo | Depende de | Quién lo sabe | Texto previsto |
|---|---|---|---|---|---|
| E1 | Plan de nuevas casas: quién recibe una y quién no. Zorro lo nota. | FLEXIBLE | — | Colonia entera | Relato de Zorro |
| E2 | Nuevo templo: Kliff lo decide tras la ausencia de fe de los demás o tras una señal personal (ver **Q8**). | ANCLA | — | Kliff; colonia | Diario de Kliff + bitácora |
| E3 | Túneles: se excavan entre zonas de la base. Pueden servir para defensa, huida o secreto. | FLEXIBLE | — | Ina, Lexington, quien dirija | Nota de Ina (su primera voz, breve) |
| E4 | Un túnel llega más lejos de lo previsto (cueva, galería de los Ixthar, campo fúngico). Sin enemigo aún, solo señal. | RESERVA | E3 | Quien lo vea | Bitácora o escena |
| E5 | Inauguración del templo nuevo o primera ceremonia. | ANCLA | E2 | Colonia entera | Escena + nota de Zorro (escéptica) |

**Huecos del hilo:** si «nuevo templo» sustituye al actual o lo amplía; si GAPA «responde» de algún modo (**Q8**); si los túneles tienen un nombre in-world.
**Detalle a vigilar:** Lexington y Ina son los mineros; el mímico era de la excavación. El jugador comentó que sería curioso un vínculo con Lexington, pero **no hay ninguno establecido**.

#### Hilo F · El viaje de Kliff (donde obtiene poderes eléctricos)

**Ya establecido:** `META`: Kliff es inmortal, con psycasts, y no lo sabe; su origen es desconocido; el Imperio lo conoce mejor de lo esperado. En el juego, el poder será eléctrico.
**Por qué es la pieza central:** saca a Kliff de la colonia justo cuando la desconfianza está en su punto más alto (relación 1), da una razón visible para que Zorro y Tarylla reaccionen a él (relaciones 2 y 3) y abre la pregunta de su origen sin responderla.

| ID | Evento | Tipo | Depende de | Quién lo sabe | Texto previsto |
|---|---|---|---|---|---|
| F1 | Kliff decide partir: un sueño, una señal de GAPA, un rumor o una necesidad concreta. Deja a Unkas al mando. | ANCLA | A1 | Colonia entera | Bitácora |
| F2 | El viaje: dónde va y qué encuentra (ver **Q7**). Pasa lejos de la colonia; su diario es la única fuente. | ANCLA | F1 | Solo Kliff | Diario de Kliff |
| F3 | El poder: cómo lo obtiene y cómo lo interpreta él (¿bendición de GAPA?, ¿castigo?, ¿fenómeno?). | ANCLA | F2 | Kliff (y un testigo posible) | Diario de Kliff |
| F4 | Vuelta de Kliff: primera vez que la colonia ve el poder. | ANCLA | F3 | Toda la colonia | Escena + bitácora |
| F5 | Consecuencias inmediatas: Zorro lo mide y lo explica; Tarylla lo ve y calla; Unkas recalcula. | ANCLA | F4 | Zorro, Tarylla, Unkas | Tres notas breves |

**Huecos del hilo:** destino, duración, acompañante (ninguno / un recién llegado / Zhethe), qué parte del poder revela sobre su origen, y si Kliff se entera en algún momento de su inmortalidad (**Q7**). Propongo que **no** en el arco 3.

#### Hilo G · Primeros indicios (pequeños) de amor Kliff + Zorro

**Ya establecido:** Zorro tiene un *crush* leve y lo oculta con sarcasmo; Kliff no ha escrito nada sobre ella aparte de «huérfana con buena mano para las plantas». En el juego ya son pareja y hay un embarazo (ambos `APLAZADO`, ver 5.3). `META`: Zorro será la primera en enfrentarse a Kliff.
**Propuesta de tono:** tensión, no romance. Atracción y choque a la vez, sin declaraciones. Los «indicios claros (pequeños)» del jugador caben bien: un gesto que ninguno comenta, una frase de más.

| ID | Evento | Tipo | Depende de | Quién lo sabe | Texto previsto |
|---|---|---|---|---|---|
| G1 | Kliff menciona a Zorro por primera vez de forma personal (no solo «la que cultiva»). | FLEXIBLE | — | Solo Kliff | Diario de Kliff |
| G2 | Un momento a solas: una conversación sobre su pasado que ninguno cuenta entera. | FLEXIBLE | — | Kliff, Zorro | Escena o relato de Zorro |
| G3 | Zorro es la única que no le teme (ver A3). Eso a Kliff le descoloca. | ANCLA | A3 | Kliff, Zorro | Diario de Kliff |
| G4 | Tras el viaje (F4), Zorro es quien le explica qué le ha pasado. El primer gesto de confianza total de Kliff en alguien. | ANCLA | F4 | Kliff, Zorro | Escena + relato de Zorro |

**Ojo con la edad:** Zorro tiene 20 años. La edad de Kliff no está definida (y es inmortal). Conviene fijar su edad aparente antes de escribir G1–G4, para no establecer una diferencia que el jugador no quiere.

### 3.4 Orden tentativo (fases en el calendario in-world de 5502)

Cada fase equivale a unos 3 trimestres de juego (ver 1.4). Es un orden, no un calendario: el juego puede alterar las fases y el plan se ajusta.

| Fase | Tramo in-world | Título | Eventos | Estado del arco |
|---|---|---|---|---|
| **1** | Marzimayo (primavera) | **Ojos abiertos** | *Ya escritos:* Kliff 5502, Tarylla #6, Zorro #5. Siguen: D1–D2 (Yuld), B1–B2 (mímico), A1 (vigilancia), E1 (casas), C1. | Se presenta la tensión sin consecuencias. |
| **2** | Junligosto (verano) | **Grietas** | A2–A3 (Unkas lo nota, Zorro se enfrenta), B3–B4 (destello y tumbas), C2–C3, E2–E3, D3–D4, G1. | Se abren las fisuras. |
| **3** | Septumbre (otoño) | **Ausencia** | F1–F3 (Kliff se va), A4 (Unkas actúa), B5 (la decisión de Tarylla), E3–E4 (túneles), D5–D6. | Kliff no está; todo avanza sin él. |
| **4** | Difebrero (invierno) | **Regreso** | F4–F5, A5–A6, B6, C4–C5, E5, G2–G4. Bitácora anual de 5502 y gancho al arco 4. | Se cierra el arco con todo abierto. |

**Variante** (si el jugador prefiere que el viaje sea más temprano): mover F a la fase 2 y dejar la fase 3 para las consecuencias (A5, B5, C4). Mi recomendación sigue siendo otoño, porque deja el invierno para el regreso, y el invierno ya es el momento dramático de esta colonia.

### 3.5 Voces y formatos (techo orientativo para todo el arco)

| Personaje | Formato | Techo | Observación |
|---|---|---|---|
| Kliff | Diario | 5-6 | Narrador poco fiable. Culto, con alguna errata. |
| Tarylla | Notas | 4-5 | Fuerte voz, entusiasta, quiebra el hilo. |
| Zorro | Relatos | 4-5 | Sarcástica, joven, inteligente aunque no tanto como cree. |
| Unkas | Notas | 2-3 | Escribe poco, lo justo. |
| Ina | Nota | 0-1 | Hoy no tiene voz. Una entrada breve puede dar mucho. |
| Zhethe | Nota | 0-1 | Idem. «Va a su bola». |
| Yuld | Carta o escena | 0-1 | Solo si hace falta. |
| Lexington / Krosswynd | — | 0 | Sin lore; no se escriben hasta que el jugador defina su origen. |
| Institucional | Bitácora anual | 1 | Autor por decidir (**Q11**). |

### 3.6 Huecos propios del arco 3 (resumen)

Los que más bloquean: **Q1** (qué es un arco), **Q2** (gancho de apertura), **Q3** (qué trama Unkas), **Q4** (tumbas), **Q7** (viaje de Kliff). Todas están en la sección 6.

---

## 4. Arcos 4 a 6 (esquema)

Aquí solo se fija **qué piezas existen y cómo se tocan**. El detalle se hará cuando se cierre el arco 3.

### 4.1 Arco 4 · el mundo llama a la puerta *(título provisional)*

**Tema propuesto:** Gapaopolis deja de ser invisible. Pasa de ser una colonia oculta a una pieza en el tablero de las demás facciones.

| Hilo | Qué es | Conecta con |
|---|---|---|
| **Las repúblicas** | La primera ronda diplomática con las tres grandes naciones. El anclaje más firme es la **visita de emisarios** (`FUTURO`, ~90 %): Kliff los recibe como representante de Gapaopolis; los de El Umbral acampan fuera de la muralla; uno viste túnica negra y «escalofriante». | Zorro (conoce los símbolos del Umbral). Ver 5.5. |
| **Los contratos de la Liga del Valor** | La Liga guía de la mano a Gapaopolis y le ofrece contratos. Encaja que sean contra bandidos y saqueadores (odia a los bandidos; Cuervo Negro es su enemigo). | Hilo D (carruaje asaltado), Yuld, Krosswynd. |
| **Las sospechas de El Umbral y la niebla** | Gapaopolis sospecha que El Umbral está detrás de la niebla. El Umbral, que hoy la desconoce, se interesa por ella. | Tarylla (esqueleto cautivo), Zorro (origen en Chapozos), mímico. |
| **Las exigencias de El Bastión** | Le ofrece «paz» gratuita, le exige reforzar filas e impone su voluntad. Quiere a Gapaopolis en la frontera con los Ixthar. | Unkas (su pasado Ixthar), Kliff (poder eléctrico). |
| **Las guerras Ixthar** | El conflicto armado con la colmena, que es enemiga del Bastión y vecina de Gapaopolis. Gapaopolis participa para ganarse el favor del Bastión. | Túneles (E4), Unkas (A, resolución). |

**Dependencias del arco 3 que hay que dejar sembradas:** los túneles hacia los Ixthar (E4), la sospecha de Kliff hacia Unkas (A6), el esqueleto cautivo (B), el poder de Kliff (F), Yuld y los bárbaros (D2).
**Preguntas abiertas:** ¿«las repúblicas» son las tres facciones o algo distinto? (5.1) · ¿las «guerras» incluyen a los bárbaros (Cuervo Negro) o son solo contra los Ixthar? · ¿cuándo se resuelve el pasado de Unkas?

### 4.2 Arco 5 · la caída del tablero *(título provisional)*

**Tema propuesto:** todos los aliados eran provisionales. Gapaopolis pasa de elegir amigos a elegir *cuál* es el mal menor.

| Hilo | Qué es | Conecta con |
|---|---|---|
| **La revelación de El Umbral** | Se descubre su naturaleza real: magia oscura, la facción oculta tras las sombras, sus planes contra El Imperio. Es «el enemigo final de esta era». | Zorro (¿huyó de allí?), Tarylla, la niebla, el emisario encapuchado. |
| **El pacto con los primeros hombres** | Alianza con los Primeros Hombres, enemigos directos de El Umbral. | Posiblemente los Exiliados o la Liga como intermediarios; Unkas. |
| **La traición de El Bastión** | El Bastión, que había involucrado a Gapaopolis en sus asuntos, se alía con El Umbral. | Las exigencias del arco 4. |
| **El trato con el diablo (El Imperio)** | El Imperio, enemigo del Umbral, interviene. `FUTURO`: el líder de la Liga dice que hay otra ficha en el tablero; **quieren a Tarylla**. | Tarylla (resolución de sus tres identidades), Kliff. |
| **La Gran Guerra Final** | `FUTURO`: Gapaopolis, los Primeros Hombres y la Liga declaran la guerra a las dos potencias; es una guerra perdida; veinte soldados imperiales llegan en un zepelín, destruyen al Umbral y al Bastión, se llevan a Tarylla, rescatan a Kliff y lo nombran Terrateniente. | Todo lo anterior. |

**Preguntas abiertas:** ¿el «trato con el diablo» es aceptado (Tarylla cedida) o Kliff lo rechaza como dice `FUTURO`? (5.4) · ¿quién cae realmente en la guerra y qué se pierde en Gapaopolis? · ¿dónde queda la inmortalidad de Kliff cuando lo «rescatan»?

### 4.3 Arco 6 · el nuevo orden *(título provisional)*

El jugador lo dejó como «ideas sueltas». Lo trato como **banco de ideas**, con una lectura tentativa de cada una:

| Idea | Lectura tentativa | Duda |
|---|---|---|
| **La grita** | ¿Un lugar, un grito de guerra, un movimiento o una facción? | No lo sé: necesito que el jugador la describa. |
| **El gremio de aventureros** | Un gremio nuevo (¿de la Liga? ¿independiente?) que surge tras la guerra. | ¿Es una facción nueva o parte de la Liga? |
| **El Imperio** | Tras la guerra, el Imperio gobierna de hecho. | ¿Gapaopolis queda como territorio imperial? |
| **Monarquía** | Podría referirse a El Imperio (base monárquica) o al título de Terrateniente de Kliff. | ¿Qué reino se funda y quién reina? |
| **Nuevas casas** | ¿Casas nobles (linajes con título) o casas construidas? Encaja con los «títulos reales» del Imperio. | ¿Es lo mismo que las «nuevas casas» del arco 3? |

**Dependencia posible:** un linaje (hijo/a de Kliff y Zorro, hoy `APLAZADO`) daría sentido a «monarquía» y «casas». No se toca hasta que el jugador lo autorice.

---

## 5. Incoherencias y tensiones detectadas

Ordenadas por el daño que harían si no se resuelven. Ninguna es un error del jugador: la mayoría son cosas que el plan ha hecho visibles.

### 5.1 «Las repúblicas» ya no existe como término
La lista del arco 4 dice «Las repúblicas», pero el jugador retiró «República» de las fichas de facciones (R26): son El Umbral, La Liga y El Bastión. Aun así, el texto de `FUTURO` de Zorro dice «república del Este» (en boca de un personaje) y su encabezado, «Imperio del Este». Hay que decidir si «repúblicas» es un término in-world coloquial o si debe sustituirse.

### 5.2 Zorro y El Umbral
Zorro es de «una civilización muy avanzada» (canon del proyecto) y, según el WIP, creció en Chapozos «a la sombra de La Aguja Solar», es decir, en territorio de El Umbral. Pero El Umbral es «Neolítico-Medieval» en la ficha. No es contradicción si los **altos secretos tecnológicos** (que sí guarda) viven en la aristocracia de la Aguja Solar, no en las aldeas: Zorro vendría de un enclave, no de «la nación». Pero es un punto que conviene fijar antes de escribir nada sobre su niñez. Además, el emisario encapuchado y escalofriante podría buscarla a ella.

### 5.3 El juego va por delante de la historia
En la partida Kliff y Zorro ya son pareja y hay dos embarazos (Zorro/Kliff y Unkas/Zhethe). El plan del arco 3 los trata como futuro. Con 1 año de historia ≈ 3 años de juego, el bebé del juego **nacerá y crecerá** antes de que la historia llegue a ese punto. Hay que decidir una norma: o se mantiene `APLAZADO` y los niños son «fondo» sin texto, o se pospone el nacimiento in-world. Mientras tanto, nada de eso puede entrar en textos.

### 5.4 El «trato con el diablo» y la negativa de Kliff
El arco 5 de Gabriel incluye «el trato con el diablo (El Imperio)». El `FUTURO` dice que Kliff **se niega** a ceder a Tarylla, va a la guerra, pierde, y El Imperio le salva y se la lleva de todos modos. Si hay *trato*, alguien cede algo; si Kliff se niega, el trato ocurre después, impuesto. Conviene decidir si el trato es una elección (Kliff acepta algo) o una derrota.

### 5.5 El evento de La Liga y los emisarios
`META` dice que El Umbral será «invitado a un evento organizado por La Liga» y se limitará a criticar a Kliff. El WIP de Zorro describe que los emisarios de las tres naciones visitan **Gapaopolis**. Son dos escenarios: ¿es el mismo evento (la Liga convoca a todos en Gapaopolis) o dos eventos distintos? Y el «intercambio cultural» del 13º–14º de Septumbre del 5501 (Kliff y Tarylla asistieron) ¿cuenta ya como el primer evento de la Liga?

### 5.6 «Carruaje» en un mundo animal-neolítico
`FUTURO` menciona un «carruaje» asaltado. La Liga es neolítica pero con «grandes carreteras»; Gapaopolis está en transición animal-neolítica. Puede encajar si es un carro de tiro, pero la palabra suena más avanzada de lo que la colonia puede nombrar. Detalle menor.

### 5.7 La carta de Yuld: «nadie la ha leído» frente a «alguien se deshizo de ella»
R7 dice que nadie ha leído la carta; `META` dice que alguien la encontró y se deshizo de ella. Quien la encontró, ¿la leyó? Si no, ¿por qué la destruyó? Es una pista narrativa buena (un colono con algo que ocultar), pero hay que dejar claro cuál de las dos afirmaciones manda.

### 5.8 Kliff y su «sin una sola desgracia»
Su diario del 1º de Marzimayo del 5502 afirma que sobrevivieron al invierno «sin una sola desgracia». Pero acaba de ver las tumbas saqueadas y a Zhethe hablar de zombis. No es error: es la negación de Kliff. Conviene mantenerlo así y que otros textos lo contradigan, no corregirlo.

### 5.9 Quién ve de verdad al enemigo
Kliff cree que Unkas habló a Zhethe de «cosas imposibles», pero Zhethe lo vio él mismo. Kliff se equivoca de culpable (ver hilo A). No es incoherencia, pero el lector solo lo sabe si la información cruza los textos de Zhethe y Unkas, y hoy Zhethe no tiene voz.

### 5.10 Nombres de archivo con `xx`
Los borradores recientes usan `5502-01-xx_…`. La convención de [`_convenciones.md`](../_convenciones.md) pide `00` para el día desconocido (`5502-01-00_…`), y el mes va de `01` a `04`. Lo corregiré al archivar.

### 5.11 «Nuevas casas» en dos arcos
La lista del arco 3 (obras) y la del arco 6 hablan de «nuevas casas». Si en el arco 6 son casas nobles, hay que evitar que el lector confunda ambas. Propongo reservar «casas» para el arco 3 (edificios) y «linajes» o «Casa» con mayúscula para el arco 6 (nobleza).

---

## 6. Preguntas que necesito del jugador

Ordenadas de más a menos urgentes. Entre paréntesis, **mi recomendación** (por defecto, si no hay preferencia).

### Para arrancar el arco 3

| # | Pregunta | Opciones | Recomendación |
|---|---|---|---|
| **Q1** | ¿Un arco equivale a un año de historia? Y ¿el arco 3 es el 5502 (arco 1 = 5500, arco 2 = 5501)? | Sí / No / Otra | **Sí.** Encaja con «nuestro tercer año» de Kliff. |
| **Q2** | ¿Qué abre el arco 3 (el «sin ideas»)? | 0a Yuld y los bárbaros · 0b Ferroespanto · 0c el mímico · otra | **0a**: ya está planeado y une varios hilos. |
| **Q3** | ¿Qué trama Unkas? | (a) Nada: es imaginario · (b) Un contrapeso a Kliff, un «consejo» discreto · (c) Un relevo del mando · (d) Protegerse a sí misma y a su futuro hijo | **(b)**, con matiz de (d): hace que Kliff tenga y no tenga razón. |
| **Q4** | ¿Quién o qué abrió las tumbas de Kaelen, Liry y Ozan? | (a) Los muertos se levantaron solos (anomalía) · (b) La Tarylla «corrompida», sin saberlo · (c) Alguien externo (necromante, Cuervo Negro, El Umbral) · (d) No se explica en el arco 3 | **(d)** con pista hacia (a) o (b). |
| **Q5** | ¿Qué pasa con el mímico? | (a) Lo encuentra y lo mata · (b) No lo encuentra: sigue libre · (c) Reaparece como algo inesperado (imitando a alguien) · (d) Queda ligado a la niebla del arco 4 | **(b)** hasta el arco 4, con un susto en el arco 3. |
| **Q6** | ¿Cómo se «abre la puerta» a la nigromancia? | (a) Por amor o duelo · (b) Por curiosidad científica · (c) Por necesidad (defensa) · y ¿cuánto lo ve el lector? | **(b)+(a)** y que el lector vea el «después», no el acto. |
| **Q7** | ¿Cómo es el viaje de Kliff? Destino, duración, acompañante, origen del poder eléctrico y cómo lo interpreta (¿bendición de GAPA?). ¿Se entera de su inmortalidad? | Abierto | Otoño; **solo**; lo interpreta como señal de GAPA; **no** se entera de su inmortalidad en este arco. |
| **Q8** | ¿El nuevo templo sustituye al actual? ¿GAPA «responde» de algún modo visible? | Abierto | Lo amplía; **sin respuesta visible** (que siga siendo duda de lector). |
| **Q9** | ¿Cuándo es la primera confrontación Zorro–Kliff y se mezcla con el indicio de amor? | Fase 2 / Fase 4 / otro | **Fase 2** (A3 y G3 a la vez). |
| **Q10** | ¿Cómo se une Krosswynd y qué relación tiene con Zorro? | (a) Con Yuld, como granjero · (b) Amigos de huerto · (c) Un rival de Kliff por Zorro · (d) Otro | **(a)+(b)**; y dejar abierta (c) sin forzarla. |
| **Q11** | ¿Quién escribe la bitácora anual de 5502? ¿Cuándo cierra el año? | Unkas / Kliff / «la colonia» (anónimo) | **Unkas**: secretaria natural y la que más tiene que callar. |

### Para más adelante (pueden esperar)

| # | Pregunta |
|---|---|
| Q12 | «Las repúblicas»: ¿son las tres facciones o algo distinto? (5.1) |
| Q13 | ¿Las «guerras» incluyen a los bárbaros (Cuervo Negro) o son solo contra los Ixthar? |
| Q14 | ¿«La grita» es un lugar, una facción, un movimiento o un grito de guerra? |
| Q15 | ¿Gapaopolis queda bajo El Imperio al final del arco 5? ¿Qué significa «Monarquía»? (arco 6) |
| Q16 | ¿El «trato con el diablo» se acepta o se rechaza? (5.4) |
| Q17 | ¿Cómo manejamos los embarazos del juego cuando la historia aún no llegó? (5.3) |
| Q18 | ¿Quién destruyó la carta de Yuld y la leyó? (5.7) |
| Q19 | ¿Cómo encaja Zorro con El Umbral y Chapozos? (5.2) |
