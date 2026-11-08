# Publicar el portafolio en GitHub Pages

Este paquete contiene una web estática completa. No tienes que programar ni instalar bibliotecas para usarla.

## 1. Crear el repositorio

1. Inicia sesión en GitHub en la cuenta `SBet18`.
2. Crea un repositorio público llamado **`sbet18.github.io`**. Debe estar en minúsculas.
3. Déjalo vacío (sin añadir README inicial), o acepta y reemplaza el README si lo creaste.

Este repositorio es **independiente** de `esp32-soil-irrigation-controller`; no modifiques el proyecto ESP32.

## 2. Subir la página

Descomprime `Engineering_Portfolio_GitHub_Pages.zip` y sube todos los archivos y carpetas que contiene a la **raíz** del repositorio nuevo. Debe existir `index.html` en la raíz, al mismo nivel que `assets/`, `projects/` y `README.md`.

La subida puede hacerse desde la web de GitHub (**Add file → Upload files**). Si GitHub no conserva la estructura de carpetas en la subida desde el navegador, utiliza GitHub Desktop o Git en el ordenador.

Alternativa con Git (en una terminal dentro de la carpeta descomprimida):

```bash
git init
git add .
git commit -m "Publicar portafolio de ingeniería"
git branch -M main
git remote add origin https://github.com/SBet18/sbet18.github.io.git
git push -u origin main
```

## 3. Activar GitHub Pages

En el repositorio, entra a **Settings → Pages**.

En **Build and deployment**, selecciona **Deploy from a branch**, rama **main**, carpeta **/(root)** y guarda.

Tu enlace público previsto será **https://sbet18.github.io/** una vez publicado. No está publicado automáticamente desde este paquete.

## 4. Verificar

- Portada: cuatro proyectos separados, experiencia, formación y contacto.
- Abaqus: PDF en inglés integrado y enlace al informe original francés.
- Fixture del monoplaza: independiente de la participación en Formula SAE eléctrico.
- Conveyor: modelos CAD, muestra física y resultado relativo a presupuesto inicial.
- ESP32: enlace al repositorio de código.
- Revisar vista en móvil y escritorio antes de usarlo en candidaturas.

## Antes de hacer público

- **BFR Systems:** confirma que puedes volver a publicar las imágenes y la descripción de ese proyecto industrial en una web pública.
- **Informe Abaqus en francés:** aparecen nombres de compañero y docente. Confirma si puedes hacerlo público; si no, elimina `assets/reports/FEA_Convergence_Original_FR.pdf` y también su enlace desde `projects/abaqus-mesh-convergence.html`.
- **Datos personales:** el CV completo y el teléfono no se incluyen en la web. El contacto por correo usa el correo académico facilitado en el CV; puedes eliminarlo de `index.html` si lo prefieres.
- **Resultados:** el 0,394 % del estudio Abaqus es una diferencia relativa respecto a la malla anterior, no un error absoluto; el 63 % del conveyor compara presupuestos, no costes totales.

## Cambios futuros

Puedes abrir los archivos `.html` con cualquier editor de texto y cambiar los párrafos. Para imágenes, añade o reemplaza archivos en `assets/img/`. La apariencia general está en `assets/css/styles.css`.
