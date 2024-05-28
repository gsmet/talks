## Quarkus GitHub Action

* Our newest addition
* Same but for GitHub Actions
* Tons of features to make the development of GitHub Actions  in Java easier
* Fully documented (again!): https://docs.quarkiverse.io/quarkus-github-action/dev/ !

-

## Create an action

```
quarkus create app \
    -x io.quarkiverse.githubaction:quarkus-github-action \
    org.acme:my-github-action:999-SNAPSHOT \
    --name="My Action" \
    --description="Description of my action" \
    --data=github-action-codestart.github-repository=org/my-github-action
```

-

## Implement your action

```java
public class MyAction {

    @Action
    void action(@Issue.Opened GHEventPayload.Issue issuePayload,
            Inputs inputs, Commands commands) throws IOException {
        issuePayload.getIssue().comment("Hello " + inputs.getRequired("who"));

        commands.appendJobSummary("# Hello " + inputs.getRequired("who")
                + "\n\n:wave:");
    }
}
```

-

## Publish your action

* Push the repository to GitHub
* Automagically published
* That's all, folks!

-

## Use your action

```yaml
- name: Run action
  uses: org/my-github-action@main
  with:
    who: JCon Slovenia
    github-token: ${{ secrets.GITHUB_TOKEN }}
```
