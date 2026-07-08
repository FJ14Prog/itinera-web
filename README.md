# Itinera Web

Web estatica d'Itinera, un programa d'autoconeixement, habilitats i orientacio per a joves.

El projecte esta pensat per publicar-se directament com a site estatic, per exemple amb GitHub Pages.

## Contingut

- Pagina principal en catala i castella.
- Selector d'idioma amb persistencia a `localStorage`.
- Apartat de propers cursos i inscripcions obertes.
- Descarrega de dossier en catala i castella.
- Seccions de programa, metodologia, modalitats, equip, testimonis i contacte.

## Estructura

```text
.
+-- index.html
+-- styles.css
+-- script.js
+-- assets/
    +-- docs/
    |   +-- ITINERA_DOSSIER_CAT.pdf
    |   +-- ITINERA_DOSSIER_CAST.pdf
    +-- img/
        +-- anna-llacher.png
        +-- carolina-llacher.jpg
        +-- carolina-llacher.png
        +-- itinera-a.png
        +-- itinera-logo.png
```

## Desenvolupament local

No cal instal.lar dependencies. Es pot obrir `index.html` directament al navegador.

Si es vol provar amb servidor local:

```powershell
python -m http.server 8000
```

I obrir:

```text
http://localhost:8000
```

## Idiomes

Els textos traduibles estan marcats a `index.html` amb `data-i18n`.

Les traduccions i configuracions per idioma es gestionen a `script.js`:

- `translations.ca`
- `translations.es`
- `pageSettings.ca`
- `pageSettings.es`

Quan s'afegeix un text nou a la pagina, cal afegir la mateixa clau al diccionari de catala i castella.

## Assets

Les imatges es troben a `assets/img`.

Els dossiers descarregables es troben a `assets/docs`.

La foto optimitzada que fa servir la web per a Carolina es `assets/img/carolina-llacher.jpg`.
El PNG original es conserva com a font.

## Publicacio

El projecte es publica des de la branca `main` del repositori:

```text
https://github.com/FJ14Prog/itinera-web
```

Si GitHub Pages esta activat, els canvis pujats a `main` es desplegaran segons la configuracio del repositori.
