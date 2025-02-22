# Contributing

## Guidelines

* **Node 18 LTS:** Homebridge projects have (if not stated otherwise) a minimum Node version requirement of 18.15.0.
  Pull requests MUST NOT require a Node version greater than that unless the feature is
  enabled/backported via [TypeScript][link-typescript]. If a higher version requirement may be justified 
  you SHALL include your reasoning in the pull request discussion.

* **Coding Standard:** Linting errors are checked by [ESLint][link-eslint].  
  Keeping a consistent style throughout the codebase keeps the cognitive load low for all
  contributors and keeps the code style homogeneous.

* **Add tests:** All pull requests SHOULD include unit tests to ensure the change works as
  expected and to prevent regressions.
  Any pull request containing a bug fix SHOULD include a regression test for the given fix.

* **Document any change in behaviour:** Homebridge projects rely on inline documentation 
  powered by [TypeDoc][typedoc-formatting].  
  Additionally, some projects MAY rely on GitHub Wikis which MIGHT need to be updated.

* **Consider our release cycle:** Before creating any pull request, please read through our concept for 
  [release cycles][release-cycle]. Most notably the section explaining our [Git Workflow][git-workflow].

* **One pull request per feature:** If you want to do more than one thing, send multiple pull requests.
  Otherwise, your pull request could be rejected.

* **Send coherent history:** Make sure each individual commit in your pull request is meaningful.
  If you had to make multiple intermediate commits while developing,
  please [rebase or squash them][link-git-rewrite] before submitting.

## Running tests

In order to contribute, you'll need to check out the source from GitHub and
install dependencies using npm:

```bash
git clone https://github.com/homebridge/<PROJECT>.git
cd <PROJECT>
npm install
npm test
```

## Reporting a security vulnerability

See [SECURITY.md](SECURITY.md)

**Happy coding**!

[link-typescript]: https://www.typescriptlang.org/
[link-eslint]: https://eslint.org/
[typedoc-formatting]: https://typedoc.org/guides/doccomments/
<!-- TODO update wiki page links, currently they point to the HAP-NodeJS repo! -->
[release-cycle]: https://github.com/homebridge/HAP-NodeJS/wiki/Release-Cycle
[git-workflow]: https://github.com/homebridge/HAP-NodeJS/wiki/Release-Cycle#git-workflow
[link-git-rewrite]: http://www.git-scm.com/book/en/v2/Git-Tools-Rewriting-History#Changing-Multiple-Commit-Messages
