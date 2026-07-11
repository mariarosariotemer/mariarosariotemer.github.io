# Portafolio profesional — Guía para ella (sin escribir código)

Esta página web está pensada para actualizarse **desde la página web de GitHub**,
sin instalar nada y sin utilizar comandos. La página muestra sus
investigaciones y análisis en formato **PDF** (no fotos de obras), pensada para una
estudiante de Mercado del Arte / Negocio del Arte.

## Estructura

```
portfolio/
├── index.html      ← la página (textos + lista de investigaciones)
├── images/
│   └── profile.jpg  ← foto de perfil (sección «Acerca de»)
├── papers/          ← aquí van los PDF de investigaciones, análisis y casos prácticos
└── cv/
    └── cv.pdf       ← el currículum en PDF
```

## 1. Cómo modificar los textos (nombre, biografía, datos de contacto)

1. Ve a la página del repositorio en github.com.
2. Abre `index.html` y haz clic en el icono con forma de lápiz («Edit this file»).
3. Utiliza **Ctrl+F** (o Cmd+F en Mac) para encontrar rápidamente el texto que
   quieres cambiar. Puntos útiles que debes buscar:
   - `Jane Doe` → nombre (aparece 2 veces)
   - `Art Market Analysis` → línea debajo del nombre
   - `I research and write about...` → texto introductorio
   - `I'm a final-year student...` → los dos párrafos de la sección «About»
   - `[email protected]` → correo electrónico (aparece 2 veces)
   - `instagram.com/tu nombre de usuario`, `linkedin.com/in/tu nombre de usuario` → enlaces a redes sociales
4. Modifica solo el texto entre `>` y `<` (no toques las etiquetas HTML con los
   corchetes angulares).
5. Al final de la página, haz clic en **«Commit changes»** para guardar.

**Consejo:** haz un cambio cada vez y comprueba la página web después de
cada vez que guardes los cambios.

#

Traducción realizada con la versión gratuita del traductor DeepL.com
