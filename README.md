# actions.add-npm-register

Append `//npm.pkg.github.com/:_authToken=xxxxxx` to `.npmrc`.

```yaml
name: Example
on: push

jobs:
  example:
    name: Example
    runs-on: ubuntu-latest
    steps:
      - uses: buka-inc/actions.add-npm-registry@v1
        with:
          registry: npm.pkg.github.com
          authToken: ${{ secrets.GITHUB_TOKEN }}
```
