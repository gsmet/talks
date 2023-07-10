## Quarkus GitHub Action

* Le petit dernier
* Tout pareil mais pour les GitHub Actions
* Avec plein de petites choses pour faciliter le dév Java de GitHub Actions
* Et une doc: https://docs.quarkiverse.io/quarkus-github-action/dev/ !

-

## Créer une action

```
quarkus create app \
    -x io.quarkiverse.githubaction:quarkus-github-action \
    org.acme:my-github-action:999-SNAPSHOT \
    --name="My Action" \
    --description="Description of my action" \
    --data=github-action-codestart.github-repository=org/my-github-action
```

-

## Implémenter une action

```java
public class MyAction {

    @Action
    void action(@Issue.Opened GHEventPayload.Issue issuePayload,
            Inputs inputs, Commands commands) throws IOException {
        issuePayload.getIssue().comment("Hello " + inputs.getRequired("who"));

        commands.appendJobSummary("# Hello Riviera DEV\n\n:wave:");
    }
}
```

-

## Publier l'action

* On pousse le repository sur GitHub
* Un workflow publie l'action automatiquement
* That's all, folks!

-

## Utiliser l'action

```yaml
- name: Run action
  uses: org/my-github-action@main
  with:
    who: Riviera DEV
    github-token: ${{ secrets.GITHUB_TOKEN }}
```
