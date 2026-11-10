# demo_gh_template

Holds a reusable GitHub Actions workflow: `.github/workflows/reusable-build.yml`.

Call it from another repo:

```yaml
jobs:
  build:
    uses: NyiNyiSoePaing/demo_gh_template/.github/workflows/reusable-build.yml@main
    with:
      environment: dev
    secrets: inherit
```

Private repo: Settings → Actions → General → Access must allow repos owned by the user.
