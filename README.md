# Rabearivelo

Dépôt des fichiers TEI présentés sur l'édition électronique https://rabearivelo.huma-num.fr

## Poésie 
 - Poèmes épars en malgache
 - Sary-Nofy / Presque-Songes
 - Nadika tamin’ny alina / Traduit de la nuit

En plus des fichiers TEI, ce dépôt contient les textes sans l’apparat critique au format Markdown Pandoc avec usage de l’extension [`raw_text`](https://pandoc.org/MANUAL.html#extension-raw_tex) pour les marques de fin de ligne.

À partir des fichiers `.md` on peut générer :
 - des fichiers `.docx` `pandoc -f markdown -t docx --lua-filter=src/pagebreak.lua presque-songes.md -o presque-songe.docx`
 - des fichiers `.pdf`  `pandoc -f markdown -t pdf -s -V papersize:a4 --lua-filter=src/pagebreak presque-songes.md -o presque-songes.pdf