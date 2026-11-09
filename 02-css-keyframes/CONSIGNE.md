# Exercice de départ — 02-css-keyframes

Ce dossier correspond strictement à `02-Demos/02-css-keyframes/etape-00/`.

Objectif : suivre les étapes de la présentation et faire évoluer les fichiers sans utiliser le corrigé.

Pour Vue (`08-` et `09-`) : `npm install`, puis `npm run dev`. Pour GSAP HTML : connexion Internet nécessaire (CDN).


## Comment fonctionne l'animation
### Le HTML
Dans index.html:15, un simple 
<div class="card badge-demo">Nouveau message</div>. 

Il a deux classes. `card` donne l'apparence (fond bleu, coins arrondis) et `badge-demo` déclenche l'animation.

### Le CSS
1. Les keyframes (style.css:76-86) définissent l'animation nommée pop :

```css
@keyframes pop {
    from { transform: scale(.96); opacity: .6 }
    to   { transform: scale(1.05); opacity: 1 }
}
```

- État de départ : légèrement rétréci (96 %) et semi-transparent (60 %).
- État d'arrivée : légèrement agrandi (105 %) et totalement opaque.