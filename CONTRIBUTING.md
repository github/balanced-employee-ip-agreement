## Contributing

Hi there! We're thrilled that you'd like to contribute to the Balanced Employee IP Agreement (BEIPA). Your help is essential. Our [README](README.md) describes the project, its purpose, and caveats, and is necessary reading for contributors.

Contributions to this project are released to the public domain under [CC0-1.0](LICENSE.md).

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

## Help wanted

Browse [open issues](https://github.com/github/balanced-employee-ip-agreement/issues) to see current requests. We also generally want to hear about:

* Legal issues with BEIPA (e.g., how it works in different jurisdictions)
* Typos
* Clearer wording
* Companies using BEIPA
* Translations
* Other employee IP agreements that have been open sourced

[Open an issue](https://github.com/github/balanced-employee-ip-agreement/issues/new) to tell us about any of the above. You may also open a pull request to propose specific changes, but it's always OK to start with an issue.

Substantive questions about and suggestions for BEIPA are welcome. We'll try to acknowledge them promptly, but may take a long time to respond on the substance, if we can. GitHub uses a version of the agreement, so our communication about it and direction for its development must be carefully considered. Also, remember that such communication [is not legal advice and comes without warranty](README.md#disclaimer).

## Versioning

BEIPA applies MAJOR.MINOR.PATCH [semantic versioning](http://semver.org/) to its domain as follows:

1. MAJOR version when objectives of agreement change. A company using BEIPA would have to fully evaluate a new major version to determine fit.
2. MINOR version when agreement changes do not change objectives of agreement but are substantial enough to merit legal scrutiny from any user.
3. PATCH version for corrections which any user would likely want to accept with minimal additional review.

Any change to the agreement text mandates a new version. Before merging any change to the agreement to master, a maintainer will:

1. Have changes reviewed by GitHub Legal.
2. Update version number in the agreement title/heading and commit to branch to be merged.
3. Merge branch with new version.
4. Tag and push: `git tag vx.x.x; git push --tags`
5. Create docx, odt, and pdf copies of the agreement:
  ```
  pandoc --smart -f commonmark Balanced_Employee_IP_Agreement.md -o Balanced_Employee_IP_Agreement.docx
  pandoc --smart -f commonmark Balanced_Employee_IP_Agreement.md -o Balanced_Employee_IP_Agreement.odt
  pandoc --latex-engine=xelatex --smart -f commonmark Balanced_Employee_IP_Agreement.md -o Balanced_Employee_IP_Agreement.pdf
  ```
6. Make a [release](https://help.github.com/articles/creating-releases/) from the tag created above, adding the docx, odt, and pdf copies as binary attachments.
7. https://github.com/github/balanced-employee-ip-agreement/releases/latest will show the release just made.

This process may become more involved if and when required by translations, support for additional jurisdictions, or desire to have old versions available in source tree, rather than only in history. At this time it is not necessary to design these procedures before they are needed.

## Resources

- [Contributing to Open Source on GitHub](https://guides.github.com/activities/contributing-to-open-source/)
- [Using Pull Requests](https://help.github.com/articles/about-pull-requests/)
- [GitHub Help](https://help.github.com)
