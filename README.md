<div align="center">

# rickyedit — sitio web personal (no oficial)

![Astro](https://img.shields.io/badge/astro-%232C2231.svg?style=for-the-badge&logo=astro&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)

Web personal **no oficial** del creador de contenido **RickyEdit**. Hecha con Astro + Tailwind CSS v4.

<a href="https://rickyedit.pages.dev/">
  <img src="https://img.shields.io/badge/☁_VER_SITIO_EN_VIVO-FF7043?style=for-the-badge&logoColor=white" alt="Demo en vivo" />
</a>

</div>

## Secciones

- **ChatGPT UI** — Interfaz tipo chat con mensaje simulado, input de texto y botones de acción rápida (Adjuntar, Buscar, Estudiemos, Crear imagen).
- **Vídeo más reciente** — Reproductor embebido con la lista de subidas de YouTube.
- **Sobre rickyedit** — Biografía con datos reales: 3.4M suscriptores YouTube, 1.3M seguidores Twitch, etc.
- **RickyEdit en datos** — Tarjetas con estadísticas reales animadas al hacer scroll (IntersectionObserver).
- **Redes sociales** — Enlaces a YouTube, Twitch, Twitter, Discord, Instagram, WhatsApp y TikTok.
- **Spotify** — Reproductor embed de música.
- **Elige una carta** — Mini-juego interactivo de selección de cartas.

## Stack tecnológico

| Capa | Tecnología |
|------|-----------|
| Framework | Astro 5 |
| Estilos | Tailwind CSS 4 |
| Fuente | Onest Variable |
| Gestor de paquetes | pnpm |
| Alojamiento | Cloudflare Pages |

## Seguridad

- Content-Security-Policy vía `<meta>` (solo permite YouTube y Spotify como orígenes externos)
- `X-Frame-Options: DENY`, `X-Content-Type-Options: nosniff`, `Referrer-Policy`, `Permissions-Policy` vía `_headers`
- `sandbox` en todos los iframes (YouTube, Spotify)
- `rel="noopener noreferrer nofollow"` en todos los enlaces externos

## Accesibilidad

- Roles ARIA y `aria-label` en componentes interactivos
- Soporte de teclado en el juego de cartas (Enter/Espacio)
- Etiquetas semánticas HTML5 (`<main>`, `<section>`, `<footer>`)
- Atributos `alt` descriptivos en imágenes
- Meta tags OG y Twitter Cards completos
- Enlace canónico

## Desarrollo

```bash
pnpm install
pnpm dev       # servidor de desarrollo
pnpm build     # build producción → dist/
pnpm preview   # previsualizar build
```

---
Hecho con ❤️ por y para la comunidad de rickyedit. Este es un sitio **no oficial**.
