# Escuela de Guardianes — Wireframe y Requerimientos Funcionales

## Sistema de Navegación

- **Móvil**: Tab bar inferior (5 tabs)
- **Desktop**: Sidebar izquierda con labels expandidas
- **Tabs**:
  1. **El Claro** (Dashboard) — icono: claro/sol entre árboles
  2. **Mi Cuidador** (Player Page) — icono: silueta con farol
  3. **Sendas** (Módulos) — icono: sendero bifurcado
  4. **Encuentros** (Comunidad) — icono: grupo/hoguera
  5. **Más** — icono: brújula (acceso a sendas secundarias, ajustes, herramientas)

---

## Pantallas

### 1. El Claro (Dashboard)

**Propósito**: Centro de control del Cuidador — visión general del progreso, contexto narrativo, acciones rápidas y estado del bosque.

**Secciones**:
- **Banner del Maestro Guardián**: mensaje narrativo del guía contextual al progreso actual del Cuidador + avatar del Maestro Guardián. Ejemplos: "La Niebla Gris retrocede cuando el criterio avanza", "Tu refugio tiene una nueva pieza. Sigue construyendo."
- **Estado del Cuidador**: avatar del héroe con rango actual + anillo de progreso circular mostrando Raíces actuales / Raíces necesarias para siguiente rango. Nombre del rango visible (ej: "Vigía del Bosque").
- **Senda activa**: card de la senda en curso (continuar donde lo dejó). Muestra nombre de la senda, animal salvaje asociado, progreso (ej: "3/8 pasos despejados"), botón "Continuar senda".
- **Marcas recientes**: últimas Marcas del Bosque obtenidas (logros) — máximo 3 visibles con scroll horizontal.
- **Vigilia**: contador de días consecutivos de actividad (racha) con indicador visual (llama/farol).
- **Estadísticas rápidas**: grid con métricas clave — Sendas despejadas, Raíces totales, Posición en Vigías, Herramientas obtenidas.
- **Encuentros destacados**: preview del próximo Encuentro del Bosque (mentoría, sesión especial, evento comunidad) si hay alguno programado.

**Elementos de gamificación**:
- Contador de Raíces (XP) visible en header o banner
- Insignia del rango actual
- Contador de Vigilia (streak)
- Preview del próximo hito (siguiente Marca del Bosque o rango)

---

### 2. Mi Cuidador (Player Page)

**Propósito**: Perfil del Cuidador y hub de progresión personal.

**Secciones**:
- **Avatar y rango**: visualización del personaje en su estado actual de evolución + nombre del rango + Raíces totales. El avatar evoluciona visualmente con cada rango (farol más brillante, más herramientas, aura más definida).
- **Resumen de stats**: Raíces totales, rango actual, sendas completadas, días de Vigilia, Piezas del Refugio obtenidas.
- **Línea de evolución**: timeline visual del viaje a través de los 5 rangos. Marca el rango actual y muestra los anteriores (completados) y futuros (bloqueados). Cada rango muestra su nombre y su descripción breve.
- **Galería de Marcas del Bosque**: todas las insignias/logros obtenidos, organizados por categoría (sendas, comunidad, especiales, secretas). Las no obtenidas aparecen en silueta con "?" o descripción misteriosa.
- **Colección de Huellas**: las huellas de animales salvajes identificadas. Agrupar por animal — al completar todas las huellas de un animal, se desbloquea su "perfil" con lore extendido.
- **Piezas del Refugio**: certificaciones e hitos significativos visualizados como piezas de una construcción.
- **Acceso a ajustes**: enlace a configuración del perfil.

---

### 3. Sendas (Módulos — Curso Principal)

**Propósito**: Camino de formación principal con estructura narrativa. Cada senda es un capítulo del viaje donde el Cuidador aprende a enfrentar un animal salvaje.

**Secciones**:
- **Mapa de sendas**: visualización tipo camino/mapa del bosque con las 6 sendas principales conectadas. Cada senda muestra:
  - Número y nombre (ej: "Senda 1: Fundamentos")
  - Animal salvaje asociado (ej: Lobo del Miedo) con su icono/silueta
  - Estado: bloqueada / activa / despejada
  - Progreso: barra o fracción (ej: "5/8 pasos despejados")
  - La Niebla Gris cubre visualmente las sendas bloqueadas
- **Senda expandida** (al seleccionar una senda):
  - Descripción narrativa de la senda
  - Descripción del animal salvaje que la habita
  - Lista de pasos (lecciones) dentro de la senda
  - Cada paso muestra: título, duración estimada, estado (pendiente/en curso/completado)
  - "Herramientas del Claro" asociadas a la senda (descargables)
  - Desafío final: prueba/quiz/ejercicio que simboliza "despejar" al animal salvaje
- **Indicador de Niebla Gris**: las sendas no desbloqueadas aparecen cubiertas por la niebla visualmente, creando tensión narrativa y motivación.

---

### 4. Sendas Secundarias (Cursos Adicionales)

**Propósito**: Formaciones complementarias fuera de la narrativa principal — especializaciones, talleres, contenido extra.

**Secciones**:
- **Grid de sendas secundarias**: cards con imagen de portada, título, tipo de senda (formación, especialización, acompañamiento), duración estimada, estado de progreso.
- **Filtros por tipo**: formación, certificación, acompañamiento, especialización.
- **Indicador de progreso**: por senda secundaria.
- **Tags**: dificultad (introductorio/intermedio/avanzado), temática, duración.
- **Nuevas sendas**: sección destacada para contenido recién publicado.

---

### 5. Encuentros del Bosque (Comunidad)

**Propósito**: Espacio social, de conexión y construcción colectiva entre Cuidadores.

**Secciones**:
- **Feed de actividad**: últimas acciones de la comunidad — Marcas obtenidas por otros, nuevos Guardianes del Claro, mensajes compartidos.
- **Los Vigías (Leaderboard)**: ranking de Cuidadores por Raíces. Filtros: semanal / mensual / histórico. Muestra posición propia siempre visible. Top 10 destacado.
- **Encuentros programados**: próximas mentorías, sesiones especiales, eventos. Card con fecha, tema, facilitador y botón de inscripción.
- **El Refugio colectivo**: visualización del refugio que se construye entre todos. Cada Pieza del Refugio aportada por un Cuidador se refleja aquí. Muestra cuántas piezas lleva el refugio y quiénes han contribuido.
- **Hilos de conversación**: foro/tablón para compartir experiencias, dudas y buenas prácticas.

---

### 6. Onboarding

**Propósito**: Secuencia de bienvenida que introduce el universo de la Escuela de Guardianes y prepara al Cuidador para su viaje.

**Flujo**:
1. **Pantalla de bienvenida**: vista cinematográfica del bosque — una panorámica entre los árboles con luz filtrándose. Texto: "Bienvenido a la Escuela de Guardianes. El bosque te espera." Botón: "Adéntrate en el bosque".
2. **Presentación del Maestro Guardián**: el guía se presenta. "Soy el Maestro Guardián. Conozco este bosque, sus senderos y sus amenazas. Mi misión es acompañarte." Entrega simbólica de los tres objetos (mapa, brújula, refugio).
3. **Introducción a la misión**: breve explicación del rol del Cuidador, la Niebla Gris y los animales salvajes. "La Niebla Gris avanza cuando falta claridad. Tu misión es despejarla."
4. **Primer vistazo a la primera senda**: preview de la Senda 1 y el Lobo del Miedo. "Tu primer desafío te espera. ¿Estás listo para comenzar?"
5. **Tooltips en El Claro**: tour guiado del Dashboard con tooltips señalando cada sección clave.

**Overlays y Tooltips**:
- **Primer login**: tour guiado con tooltips sobre las secciones principales del Claro
- **Marca del Bosque desbloqueada**: overlay celebratorio con la insignia, su nombre y un texto narrativo del Maestro Guardián
- **Subida de rango**: overlay de evolución — el avatar cambia, el farol brilla más, mensaje especial del Maestro Guardián. "Has dejado de ser Cuidador de Sendas. Ahora eres Vigía del Bosque."
- **Nueva senda desbloqueada**: teaser narrativo — se disipa la niebla de esa senda, se revela el animal salvaje que la habita
- **Pieza del Refugio**: animación de la pieza encajando en el refugio colectivo

---

## Sistema de Notificaciones

| Evento | Mensaje (voz del Maestro Guardián) |
|---|---|
| **Marca desbloqueada** | "Has dejado una nueva marca en el bosque. [Nombre de la marca]" |
| **Subida de rango** | "Tu farol brilla con más fuerza. Ahora eres [nuevo rango]." |
| **Nuevo contenido** | "Una nueva senda se abre en el bosque. Adéntrate y descubre qué te espera." |
| **Recordatorio de Vigilia** | "El bosque te espera, Cuidador. No dejes que la Vigilia se apague." |
| **Comunidad** | "Un compañero del bosque ha compartido algo. Acércate al Encuentro." |
| **Pieza del Refugio** | "Has añadido una nueva pieza al Refugio. La red se fortalece." |

---

## Resumen de Mecánicas de Gamificación

| Mecánica | Implementación | Nombre en el Universo |
|---|---|---|
| XP | Puntos por paso completado, quiz, actividad, participación | **Raíces** |
| Rangos | 5 niveles con evolución visual del avatar y farol | **Rangos de Guardián** (Joven Cuidador → Guardián del Claro) |
| Logros | Insignias por hitos, sendas completadas, participación | **Marcas del Bosque** |
| Racha | Contador de días consecutivos de actividad | **Vigilia** |
| Leaderboard | Ranking semanal/mensual por Raíces | **Los Vigías** |
| Desafíos | Enfrentamientos simbólicos con animales salvajes al final de cada senda | **Desafíos del Bosque** |
| Coleccionables | Huellas de animales salvajes para desbloquear lore | **Huellas** |
| Certificaciones | Hitos visualizados como piezas de construcción | **Piezas del Refugio** |
| Descargables | Guías, plantillas, checklists | **Herramientas del Claro** |
| Progresión narrativa | Disipación visual de la Niebla Gris al avanzar | — (visual, no mecánica) |

---

## Pantallas Extra (si aplica)

- **Perfil del Animal Salvaje**: se desbloquea al coleccionar todas sus huellas. Muestra lore extendido, qué representa, consejos del Maestro Guardián para reconocerlo en la práctica profesional real.
- **El Refugio** (vista completa): visualización detallada del refugio colectivo con todas las piezas aportadas por la comunidad. Posibilidad de ver quién contribuyó cada pieza.
- **Herramientas del Claro** (biblioteca): acceso organizado a todos los descargables obtenidos, filtrados por senda/temática.
