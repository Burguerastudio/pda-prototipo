# Escuela de Guardianes — PDA Bullying

## URLs
- **Repo**: https://github.com/Burguerastudio/pda-prototipo
- **Vercel**: https://pda-prototipo.vercel.app
- **Key visuals**: https://pda-prototipo.vercel.app/key-visuals/

## Stack
- **Key visuals**: Nano Banana 2 (imagenes) + HTML/CSS (presentacion)
- **Diseno de pantallas**: Google Stitch (pendiente Fase 2)
- **Desarrollo**: Astro + Tailwind CSS (pendiente)
- **Deploy**: Vercel
- **Assets**: Nanobanana / Gemini (gemini-3.1-flash-image-preview)

## Estructura del Proyecto

```
├── docs/
│   ├── CLAUDE.md          ← este archivo
│   ├── DESIGN.md          ← placeholder (se genera en Fase 2)
│   ├── NARRATIVE.md       ← universo, personajes, tono, vocabulario
│   ├── WIREFRAME.md       ← requerimientos funcionales por pantalla
│   ├── ASSETS.md          ← inventario de imagenes
│   └── ASANA.md           ← plan de proyecto
├── references/
│   ├── GUIA-REFERENCIAS.md
│   ├── INDEX.md
│   └── [subcarpetas con imagenes de referencia]
├── key-visuals/
│   ├── index.html         ← presentacion de direcciones visuales
│   └── img/
│       ├── a/             ← imagenes direccion A
│       ├── b/             ← imagenes direccion B
│       └── tex/           ← texturas de cards
├── src/                   ← proyecto Astro (pendiente)
└── .stitch/               ← archivos Stitch (pendiente)
```

## Estado Actual

1. ✅ `sepia-setup` — docs/ generados (CLAUDE, NARRATIVE, WIREFRAME, ASSETS, DESIGN placeholder, ASANA)
2. ✅ `sepia-references` — 26 imagenes descargadas + INDEX.md con links manuales
3. ✅ `sepia-design` Fase 1 — key visuals generados y desplegados en Vercel
4. ⏳ Esperando que el cliente elija direccion visual (A o B)
5. ⬜ `sepia-design` Fase 2 — dashboard completo (tras eleccion del cliente)
6. ⬜ Resto de pantallas, assets, desarrollo, deploy

## Direcciones Visuales Presentadas

**Direccion A — El Bosque Profundo**: dark UI, azul noche + ambar farol, Playfair Display, glassmorphism angular, ornamentos geometricos
**Direccion B — El Claro Iluminado**: light UI, crema pergamino + verde bosque, Lora, bordes cosidos, ornamentos botanicos

## Convenciones

- Lenguaje en UI: **siempre usar vocabulario del bosque** (ver NARRATIVE.md)
- Imagenes: WebP, quality 85-88
- Texturas: 512x512 minimo
- Todo el texto en espanol, nunca ingles ni Lorem ipsum

## Contexto

**Cliente**: PDA Bullying
**Agencia**: Sepia Creativa
**Tipo**: Academia online gamificada con narrativa inmersiva
**Universo**: Bosque realista-simbolico — nunca infantil
**Publico**: Profesionales en prevencion de violencia
**Tono**: Profesional, cercano, simbolico, sereno, esperanzador
