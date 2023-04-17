## Automatisation vs petites tâches

* Les petites tâches s'additionnent
* L'automatisation fluidifie le travail
* Quarkus GitHub App et Quarkus GitHub Action peuvent aider, rapidement et facilement
* Commencez petit, poussez en production, et ajoutez des fonctionnalités après

@Notes:

* [...]: with a large enough project, even small inconveniences can really slow you down
* [...]: it's a chance to offload plenty of small (or not so small) tasks
* [...]: familiar environment and no boilerplate,
  so you don't spend more time on automation than you would have manually.
* Also means even a small GitHub app is worth it: you can start small [...]

-

## Des extensions ?

* Très peu de code à maintenir
* Tout est câblé durant le build avec du code généré par Gizmo
* Quarkus extensions FTW!

@Notes:

* [...] Quarkus is all about: making your life easier
* [...] develop extensions like this one

-

## Merci de votre attention !

![](https://imgs.xkcd.com/comics/automation.png)

https://xkcd.com/1319/

-

## Ressources

* Quarkus - <https://quarkus.io>
* Quarkus GitHub App - <https://github.com/quarkiverse/quarkus-github-app>
* Documentation - <https://quarkiverse.github.io/quarkiverse-docs/quarkus-github-app/dev/>

* Cette présentation - <https://talks.smet.org/2023-04-automatisation-github-quarkus-lyon-jug/>
* Démo - <https://github.com/gsmet-bot-playground/github-automation-with-quarkus-demo-app>
* <a href="?print-pdf">Exporter les slides in PDF</a> <small>(nécessite Chrome)</small>

-

<!-- .element data-visibility="uncounted" -->

## Architecture

![](images/architecture.png)

-

<!-- .element data-visibility="uncounted" -->

## Quarkus 3

* Jakarta EE 10
* Eclipse MicroProfile 6
* Hibernate ORM 6
* Nouvelle Dev UI
* Upgrade automatisé
* Plugins pour le Quarkus CLI
* Et tout un tas d'autres trucs...

-

<!-- .element data-visibility="uncounted" -->

### Licences

Les logos dans cette présentation sont des marques déposées de leurs propriétaires respectifs aux Etats-Unis et dans d'autres pays.

Le copyright du comic strip "Automation" dans le slide "Merci de votre attention !" est propriété de Randall Munroe (author of [xkcd](https://xkcd.com/1319/)),
qui autorise l'utilisation de ce comic strip sous la [licence Creative Commons Attribution-NonCommercial 2.5](https://creativecommons.org/licenses/by-nc/2.5/).

Le reste de cette présentation est distribuée sous CC-BY-4.0.
Se reporter à https://creativecommons.org/licenses/by/4.0/ pour plus de détails.

Le code source de cette présentation est accessible à l'adresse https://github.com/gsmet/talks/.
