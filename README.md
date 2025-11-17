# Bulínova skripta z NAIL062 VaPL – vylepšená verze

[PDF dostupné na Matfyz Wiki](https://wiki.matfyz.cz/NAIL062/skripta-vapl-lepsi.pdf).

## Změny
- Odstraněna nadbytečná kapitola Úvod do logiky
- Přidány seznamy definic a vět
- Možnost exportu do A5

Vše v `/lecture/skripta/`.

## Kompilace
```sh
pdflatex skripta.tex && pdflatex skripta.tex
```

Pokud náhodou potřebujete seznam literatury (obsahující jednu knihu): `bibtex skripta`

## Export A5
Vhodné do čtečky. Místy špatně vyrenderované. [PDF na Matfyz Wiki](https://wiki.matfyz.cz/NAIL062/skripta-vapl-lepsi-a5.pdf).

`skripta.tex`:
```diff
- \documentclass[11pt,a4paper]{report}
+ \documentclass[11pt,a5paper]{report}
```

`hlavicka.tex`:
```diff
-\usepackage{a4wide}
+\usepackage[top=0.8in,bottom=0.8in,left=0.7in,right=0.7in]{geometry}
```

## Meme
![](meme.png)