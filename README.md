# groovy-linter

An example of github action for groovy/Jenkinsfile verification.

As linter the [npm-groovy-lint](https://github.com/nvuillam/npm-groovy-lint) is being used.

Verifying everything inside [pipelines](pipelines) directory.

In case of PR also github action will commnet the PR with job result.

## PR comment for successed job

```text
✅ GroovyLinter: succeeded
➡️ Open workflow job
➡️ Download job result
```

## PR comment for failed job

```text
❌ GroovyLinter: failed
➡️ Open workflow job
➡️ Download job result

❗️ Violated Rules:
Indentation violated 12 time(s)
TrailingWhitespace violated 11 time(s)
UnnecessaryGString violated 7 time(s)
SpaceBeforeOpeningBrace violated 4 time(s)
DuplicateStringLiteral violated 16 time(s)
FileEndsWithoutNewline violated 1 time(s)
```
