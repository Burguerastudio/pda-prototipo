# Escuela de Guardianes — PDA Bullying

## Stack
- **Diseño**: Google Stitch (MCP) + Stitch Skills (stitch-design, design-md, enhance-prompt)
- **Desarrollo**: Astro + Tailwind CSS
- **Deploy**: Vercel
- **Assets**: Nanobanana (generación de imágenes con IA)
- **Archivos de diseño**: Figma (solo si lo solicita el cliente)

## Estructura del Proyecto

```
├── docs/
│   ├── CLAUDE.md          ← este archivo
│   ├── DESIGN.md          ← sistema visual (generado con design-md skill)
│   ├── NARRATIVE.md       ← universo, personajes, tono, vocabulario
│   ├── WIREFRAME.md       ← requerimientos funcionales por pantalla
│   └── ASSETS.md          ← inventario de imágenes + prompts Nanobanana
├── references/            ← imágenes de inspiración visual
├── src/                   ← proyecto Astro
│   ├── components/        ← componentes reutilizables
│   ├── layouts/           ← layouts (app shell, onboarding)
│   ├── pages/             ← páginas Astro
│   ├── styles/            ← estilos globales + config Tailwind
│   └── assets/            ← imágenes generadas en Nanobanana
├── public/                ← assets estáticos
├── .stitch/               ← archivos del proyecto Stitch
└── astro.config.mjs
```

## Estrategia Responsive

- **Mobile-first**: tab bar inferior (5 tabs máximo)
- **Desktop**: sidebar izquierda con labels expandidas
- **Breakpoint**: `md` (768px) cambia entre layouts
- **Touch targets**: mínimo 44x44px en móvil
- **Safe area**: padding para iOS en tab bar

## Convenciones de Código

- Componentes Astro: PascalCase (ej: `PlayerCard.astro`)
- Tailwind: utility-first, extraer a `@apply` solo para patrones repetidos
- Colores: CSS custom properties desde tokens de DESIGN.md
- Imágenes: formato WebP, lazy loading, responsive srcset
- Animaciones: CSS transitions preferidas, JS solo para secuencias complejas
- Lenguaje en UI: **siempre usar vocabulario del bosque** (ver NARRATIVE.md)

## Flujo de Diseño

1. ✅ `sepia-setup` — estructura del proyecto generada
2. ⬜ Añadir referencias a `references/`
3. ⬜ `sepia-design` — generar key visuals e iterar pantallas en Stitch
4. ⬜ `sepia-assets` — generar prompts Nanobanana y gestionar imágenes
5. ⬜ `sepia-deploy` — migrar diseños Stitch a Astro + Tailwind

## Referencias Clave

- Universo narrativo: ver `docs/NARRATIVE.md`
- Requerimientos por pantalla: ver `docs/WIREFRAME.md`
- Sistema visual: ver `docs/DESIGN.md`
- Inventario de assets: ver `docs/ASSETS.md`
- Plan de proyecto: ver `docs/ASANA.md`

## Contexto del Proyecto

**Cliente**: PDA Bullying (Plataforma de Prevención, Detección y Actuación)
**Agencia**: Sepia Creativa
**Tipo**: Academia online gamificada con narrativa inmersiva
**Universo**: Bosque realista-simbólico — nunca infantil
**Público**: Profesionales que trabajan en prevención de violencia y complejidad emocional
**Tono**: Profesional, cercano, simbólico, sereno, esperanzador
