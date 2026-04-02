# PDA BULLYING | Escuela de Guardianes — Plan de Proyecto

## Estructura del Proyecto en Asana

Crear proyecto tipo **Board** con 6 columnas. Nombre: `PDA BULLYING | Escuela de Guardianes`

---

## 1. Setup y Documentacion

| Tarea | Prioridad | Estado |
|-------|-----------|--------|
| Recibir inputs de la agencia (narrativa, test players, storybrand) | Alta | ✅ Hecho |
| Generar docs/ con /sepia-setup | Alta | ✅ Hecho |
| Recibir test de players y storybrand oficial | Media | ⏳ Pendiente de copywriter |
| Buscar y organizar referencias visuales | Alta | 🔲 Por hacer |

**Notas**: Los inputs recibidos hasta ahora son la narrativa de marca y notas de la copy. Falta el test de players (arquetipos) y el storybrand oficial. Las referencias se organizan siguiendo `references/GUIA-REFERENCIAS.md`.

---

## 2. Diseno — Key Visuals

| Tarea | Prioridad | Dependencia |
|-------|-----------|-------------|
| Generar Direccion A en Stitch (El Bosque Profundo) | Alta | Referencias listas |
| Generar Direccion B en Stitch (El Claro) | Alta | Referencias listas |
| Presentar key visuals al cliente y elegir direccion | Alta | Direcciones A y B listas |

**Direccion A — El Bosque Profundo**: Dark UI, bosque nocturno/crepuscular, niebla, glassmorphism oscuro, acentos ambar/dorado (luz de farol). Ref: Firewatch noche + The Long Dark.

**Direccion B — El Claro**: Light/warm UI, bosque diurno con luz filtrandose, texturas papel/madera, verde bosque + dorado. Ref: Firewatch dia + cartografia vintage.

---

## 3. Diseno — Dashboard y Pantallas

| Tarea | Prioridad | Dependencia |
|-------|-----------|-------------|
| Disenar dashboard completo (desktop + mobile) | Alta | Direccion elegida por cliente |
| Disenar Mi Cuidador (Player Page) | Media | Dashboard aprobado |
| Disenar Sendas (Modulos) | Media | Dashboard aprobado |
| Disenar Secundarias + Encuentros + Onboarding | Media | Dashboard aprobado |

**Gate de aprobacion**: El cliente debe aprobar el dashboard antes de disenar el resto de pantallas. Al aprobar se genera el DESIGN.md definitivo con la skill design-md.

**Pantallas a disenar**:
- El Claro (Dashboard) — centro de control del Cuidador
- Mi Cuidador (Player Page) — perfil, evolucion, Marcas del Bosque, Huellas
- Sendas (Modulos) — mapa de 6 sendas con animales salvajes y Niebla Gris
- Sendas Secundarias — cursos adicionales fuera de la narrativa principal
- Encuentros del Bosque (Comunidad) — feed, Vigias, Refugio colectivo
- Onboarding — bienvenida al bosque, Maestro Guardian, tooltips, overlays

---

## 4. Assets — Nanobanana

| Tarea | Prioridad | Dependencia |
|-------|-----------|-------------|
| Definir estilo visual y generar prompts con /sepia-assets | Alta | DESIGN.md generado |
| Generar imagenes en Nanobanana | Media | Prompts listos en ASSETS.md |
| Integrar assets en el proyecto | Media | Imagenes generadas |

**Assets a generar (37 total)**:
- 5 rangos del Cuidador (Joven Cuidador → Guardian del Claro)
- Maestro Guardian (guia)
- Niebla Gris (villano ambiental)
- 6 animales salvajes (Lobo, Jabali, Serpiente, Cuervo, Oso, Hiena)
- 9+ Marcas del Bosque (insignias/logros)
- 6 portadas de sendas
- 8+ elementos UI (texturas, iconos, fondos)

---

## 5. Desarrollo — Astro + Tailwind

| Tarea | Prioridad | Dependencia |
|-------|-----------|-------------|
| Scaffold Astro + Tailwind con /sepia-deploy | Alta | Pantallas disenadas |
| Migrar pantallas de Stitch a componentes Astro | Alta | Scaffold listo |
| Revision responsive (mobile + desktop) | Media | Migracion completa |

**Componentes clave**:
- AppShell (sidebar desktop + tab bar mobile)
- RaicesBadge (XP display)
- RangoGuardian (badge de rango)
- VigiliaCounter (streak)
- ProgressRing (progreso circular)
- MarcaCard (logro/insignia)
- SendaCard (modulo con animal salvaje)
- AnimalSalvajeProfile (ficha de enemigo)

**Responsive**: Mobile-first, breakpoint md (768px), tab bar con safe area iOS, touch targets 44px.

---

## 6. Deploy y Entrega

| Tarea | Prioridad | Dependencia |
|-------|-----------|-------------|
| Deploy a Vercel | Alta | Responsive verificado |
| Revision del cliente + ajustes | Alta | Deploy live |
| Handoff final | Media | Ajustes implementados |

**Handoff incluye**:
- URL Vercel (produccion)
- Repo GitHub
- Figma (solo si lo piden)
- Documentacion completa en docs/

---

## Timeline Estimado

```
Semana 1  ████░░░░░░░░░░░░░░░░  Setup + Referencias
Semana 2  ░░░░████░░░░░░░░░░░░  Key Visuals + Aprobacion cliente
Semana 3  ░░░░░░░░████░░░░░░░░  Dashboard + Pantallas
Semana 4  ░░░░░░░░░░░░████░░░░  Assets Nanobanana
Semana 5  ░░░░░░░░░░░░░░░░████  Desarrollo Astro
Semana 6  ░░░░░░░░░░░░░░░░░░██  Deploy + Entrega
```

**Nota**: Timeline flexible. Las semanas de diseno pueden comprimirse o expandirse segun feedback del cliente.
