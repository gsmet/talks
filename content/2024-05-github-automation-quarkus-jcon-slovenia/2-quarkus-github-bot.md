## "Death by a thousand paper cuts"

-

## Triaging

* Constant flow of issues/pull requests
* Many components with different maintainers
* Need to ping appropriate people

-

## Affecting milestones

* Minor release every month (micro every week)
* ~ 200 issues / pull requests without milestone when releasing
* Heterogeneous team makes it harder

-

## Hard to find cause when CI fails

![](images/long-log-file.png)
![](images/complex-build.png)

-

## In one word: scale

![](images/github-activity-may-15-june-15.png)

Quarkus 3.0 = 1000+ pull requests and issues

@Notes:

We need to solve this issue. Fast.

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

* Started as a Probot bot
* Switched to Quarkus
* Went way beyond! For example...

-

## Automated triaging

![](images/triaging.png)

-

## Automated workflow

![](images/workflow.png)

-

## Automated build report

![](images/build-report.png)

-

## Annotations

![](images/build-report-annotation.png)

@Notes:

Develop how important it is for us today,
how we miss it when it’s not there,
how we are deploying it to other projects in the Quarkus ecosystem
