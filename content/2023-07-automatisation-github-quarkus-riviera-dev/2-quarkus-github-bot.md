## "Death by a thousand paper cuts"

-

## Triage

* Flux constant d'issues et de pull requests
* Beaucoup de composants avec des mainteneurs différents
* Besoin de pinger les bons interlocuteurs

-

## Affecter les milestones

* Release mineure mensuelle (micro toutes les semaines)
* ~ 200 issues / pull requests sans milestone le jour de la release
* Equipe hétérogène → process moins suivi

-

## Difficile de trouver la cause quand erreur CI

![](images/long-log-file.png)
![](images/complex-build.png)

-

## On doit aller vite

![](images/github-activity-may-15-june-15.png)

Quarkus 3 = 1000+ pull requests et issues

@Notes:

Nous devions résoudre ce problème.

Rapidement.

---

<!-- .element: class="grid" -->
## Quarkus GitHub Bot

<div class="column">

![](images/probot.png)

</div>
<div class="column" style="font-size: 4em;">

&rarr;

</div>
<div class="column">

![](images/quarkus.svg)

</div>

@Notes:

* A l'origine, un petit bot Probot
* Migration vers Quarkus
* Et on est allé beaucoup plus loin ! Par exemple...

-

## Triage automatique

![](images/triaging.png)

-

## Workflow automatisé

![](images/workflow.png)

-

## Rapport de build automatisé

![](images/build-report.png)

-

## Annotations

![](images/build-report-annotation.png)

@Notes:

Développer combien c'est important pour nous aujourd'hui,
combien il nous manque quand inactif,
et comment nous l'avons déployé sur d'autres projets dans l'écosystème Quarkus.
