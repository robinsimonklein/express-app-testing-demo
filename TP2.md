# TP2

## 1. Convention de coding

**Des commentaires (sans abus)**
Sur la plupart des projets actuels il y a trop peu de commentaires 
et on se retrouve souvent à perdre du temps à comprendre du code 
qui a été fait il y a un moment.

**Des variables correctement nommées (noms qui ont un sens)**
Je me suis déjà retrouvé sur un projet où tous singuliers étaient 
nommés au pluriel et les pluriels au singulier...

**Ajouter des CI de qualité de code en front**
Pour le moment il y a pas mal de checks de qualité de code pour les 
devs back, mais rien est fait pour le front. On pourrait ajouter un 
linter pour le js (eslint) et le css.

**Une doc claire et complète pour l'installation des projets et leur maintenance**
Il y a souvent pas suffisament de doc pour installer ou maintenir un 
projet. On se retrouve donc à devoir chercher un autre dev qui connait 
les manips pour installer un projet. Ça peut être fait avec un simple README
ou un wiki.
___
## Choix d'infrastructure
### A mettre en place :
- Stockage cloud pour prendre en compte le grossissement du nombre de 
photos donc scalable.
- BDD NoSQL pour lier des mots clés et d'autres infos aux images
- ElasticSearch pour l'indexation optimisée des datas et les 
recherches par mots clés / facettes
- Couche de sécurité pour l'accès à l'API

### Ressources :
- 1 ou 2 devs pour la partie indexation et bdd
- 1 dev pour la partie sécurité

### Coûts : 
- Cloudinary pour le stockage des photos -> ~250€/mois pour 600Go -> +3000€/an
- Amazon API Gateway -> ~20€/mois -> 240€/an
- Amazon DynamoDB -> ~5€/mois -> 60€/an
- 2 devs -> 2000€/mois -> 24000€/an
- 1 dev sécu -> 3000€/mois -> 36000€/an

**Total : 63 300€/an** 
___
## Monitoring
**WIP**
