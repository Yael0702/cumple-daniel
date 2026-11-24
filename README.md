# 🎂 Felicitación de cumpleaños para Daniel

Página web de una sola pantalla para felicitar a mi hermano Daniel por su cumpleaños. Está pensada para abrirse desde el celular y tiene un tema inspirado en sus dos gustos: la **enfermería** (su profesión) y el **dibujo**.

## Qué incluye

- **Portada** con una línea de latido (electrocardiograma) que se dibuja sola, título animado y confeti de bienvenida.
- **Globos** de colores que suben por toda la página.
- **Foto** en formato polaroid con un mensaje personal.
- **Receta médica interactiva**: Daniel marca cada indicación y, al completarlas todas, sale confeti.
- **Cuaderno de dibujos**: garabatos que se trazan al hacer scroll.
- **Música**: botón que abre la canción "Feliz cumpleaños hermano" en Apple Music.

## Tecnologías

- HTML, CSS y JavaScript puros, sin librerías ni dependencias.
- Fuentes de Google Fonts (*Caveat Brush* y *Nunito*), con fuentes de respaldo si no cargan.
- Todo en un solo archivo: la foto está incrustada en base64.

## Estructura

```
.
├── index.html   # La página completa (HTML + CSS + JS + foto)
└── README.md    # Este archivo
```

## Cómo verla

**En local:** abre `index.html` con el navegador (doble clic).

**Publicada con GitHub Pages:**

1. Sube `index.html` a un repositorio público.
2. Ve a **Settings → Pages**.
3. En **Source** elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
4. Guarda y espera uno o dos minutos. El enlace será `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Cómo personalizarla

| Qué cambiar | Dónde |
|---|---|
| Mensaje principal | Sección `#mensaje` de `index.html` |
| Indicaciones de la receta | Lista `<ul id="lista">` en la sección `#receta` |
| Frases bajo los dibujos | Sección `#dibujos`, etiquetas `<p>` |
| Canción | Atributo `href` del botón "Escuchar en Apple Music" |
| Colores | Variables CSS en `:root` al inicio de `<style>` |
| Foto | Atributo `src` de la imagen en `.polaroid` (base64 o ruta a un archivo) |

## Compatibilidad

- Probada pensando en celulares Android (Huawei, Honor) y navegadores modernos.
- Respeta la opción de **reducir movimiento** del sistema: sin globos ni animaciones si está activada.
- Soporta modo claro y oscuro.
- Si el navegador no soporta alguna animación, el contenido se muestra igual, sin efectos.

## Notas

- La música no puede reproducirse sola: Apple Music exige iniciar sesión y pulsar play. Por eso se usa un enlace que abre la app.
- El repositorio es público, por lo que cualquier persona con el enlace puede ver la foto incluida en la página.

## Autor

Hecho con cariño por su hermano ❤️
