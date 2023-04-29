
# Harmonize

## Français (French)

### Présentation

**Harmonize** est un projet *CSS* et *Sass* (avec la syntaxe *SCSS*) qui propose :
- des corrections de bugs,
- des normalisations,
- des remises à zéro et
- des styles basiques (“opinionated”).




### Intérêts

Les navigateurs Web mettent en page de façons différentes les pages Web.

Des projets ont ainsi vu le jour pour corriger ce problème :
- [Reset CSS](https://meyerweb.com/eric/tools/css/reset/) d’Eric Meyer ou encore
- [normalize.css](https://github.com/necolas/normalize.css) de Nicolas Gallagher.

Le premier adopte une approche radicale : il supprime tous les styles que les navigateurs appliquent par défaut.<br>Le second propose une méthode différente : il corrige les styles inconsistants entre navigateurs tout en gardant les styles par défauts utiles.

**Harmonize** suit la démarche de [sanitize.css](https://github.com/csstools/sanitize.css) par Jonathan Neal : il rajoute en plus des styles “opinionated”. Ce sont des styles basiques que l'on retrouve dans la quasi-totalité des projets.

Quelques exemples :
```css
*,
:after,
:before {
  box-sizing: border-box;
}
```
```css
html {
  height: 100%;
}
```
```css
body {
  min-height: 100%;
  margin: 0;
}
```
```css
img {
  max-width: 100%;
  height: auto;
}
```




### Comparaison des solutions

| Projet        | Corrections de bugs    | Normalisations         | Remises à zéro              | Styles basiques (“opinionated”)     |
| ------------- | ---------------------- | ---------------------- | --------------------------- | ----------------------------------- |
| Harmonize     | ✔️ Oui                 | ✔️ Oui, celles utiles | ✔️ Oui, celles utiles       | ✔️ Oui                             |
| sanitize.css  | ✔️ Oui                 | ✔️ Oui, celles utiles | ✔️ Oui, celles utiles       | ✔️ Oui                             |
| normalize.css | ✔️ Oui                 | ✔️ Oui, celles utiles | ✔️ Oui, celles utiles       | ❌ Non                             |
| Reset CSS     | ❌ Non                 | ❌ Non                | ✔️ Oui, **tous** les styles | ❌ Non                             |




### License

**Harmonize** utilise la [Licence MIT](https://choosealicense.com/licenses/mit/).