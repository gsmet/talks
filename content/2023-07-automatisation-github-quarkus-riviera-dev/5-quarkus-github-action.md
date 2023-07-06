## Quarkus GitHub Action

* Le petit dernier
* Tout pareil mais pour les GitHub Actions
* Avec plein de petites choses pour faciliter le dév Java de GitHub Actions
* Et [une doc](https://quarkiverse.github.io/quarkiverse-docs/quarkus-github-action/dev/index.html) !

-

## Créer une action

```
quarkus create app \
    -x io.quarkiverse.githubaction:quarkus-github-action \
    org.acme:my-github-action:999-SNAPSHOT \
    --name="My Action" \
    --description="Description of my action" \
    --data=github-action-codestart.github-repository=gsmet/my-github-action
```

-

## Implémenter une action

```java
public class MyAction {

    @Action
    void action(@Issue.Opened GHEventPayload.Issue issuePayload,
            Commands commands) throws IOException {
        issuePayload.getIssue().comment("Hello Riviera DEV");

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
  uses: gsmet/my-github-action@main
  with:
    github-token: ${{ secrets.GITHUB_TOKEN }}
```
