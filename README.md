# storybook-addon-gatsby

[![npm version][npm-version-src]][npm-version-href]
[![npm downloads][npm-downloads-src]][npm-downloads-href]
[![Github Actions CI][github-actions-ci-src]][github-actions-ci-href]
[![Codecov][codecov-src]][codecov-href]
[![Conventional Commits][conventional-commits-src]][conventional-commits-href]
[![License][license-src]][license-href]

[Storybook][storybook] addon used to load stories built with [Gatsby][gatsby].

- 🔌 One-line configuration for Storybook + Gatsby
- ✨ TypeScript support included by default

**Note**: This addon requires Storybook to be configured for Webpack 5. See the official [Storybook with Webpack 5 guide](https://gist.github.com/shilman/8856ea1786dcd247139b47b270912324) for instructions.

## Install

```bash
npm install -D storybook-addon-gatsby
```

Then include the addon to your Storybook config at `.storybook/main.js`:

```javascript
// .storybook/main.js

module.exports = {
	addons: ["storybook-addon-gatsby"],
};
```

TypeScript support is included by default, but it can be disabled with the `withTypeScript` option:

```javascript
// .storybook/main.js

module.exports = {
	addons: [
		{
			name: "storybook-addon-gatsby",
			options: {
				// Disable TypeScript support.
				withTypeScript: false,
			},
		},
	],
};
```

## Documentation

To discover what's new on this package check out [the changelog][changelog].

## Contributing

Whether you're helping us fix bugs, improve the docs, or spread the word, we'd love to have you as part of the Prismic developer community!

**Asking a question**: [Open a new topic][forum-question] on our community forum explaining what you want to achieve / your question. Our support team will get back to you shortly.

**Reporting a bug**: [Open an issue][repo-bug-report] explaining your application's setup and the bug you're encountering.

**Suggesting an improvement**: [Open an issue][repo-feature-request] explaining your improvement or feature so we can discuss and learn more.

**Submitting code changes**: For small fixes, feel free to [open a PR][repo-pull-requests] with a description of your changes. For large changes, please first [open an issue][repo-feature-request] so we can discuss if and how the changes should be implemented.

## License

```
   Copyright 2013-2021 Prismic <contact@prismic.io> (https://prismic.io)

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```

<!-- Links -->

[prismic]: https://prismic.io
[storybook]: https://storybook.js.org/
[gatsby]: https://www.gatsbyjs.com/

<!-- TODO: Replace link with a more useful one if available -->

[prismic-docs]: https://prismic.io/docs
[changelog]: /CHANGELOG.md

<!-- TODO: Replace link with a more useful one if available -->

[forum-question]: https://community.prismic.io
[repo-bug-report]: https://github.com/prismicio-community/storybook-addon-gatsby/issues/new?assignees=&labels=bug&template=bug_report.md&title=
[repo-feature-request]: https://github.com/prismicio-community/storybook-addon-gatsby/issues/new?assignees=&labels=enhancement&template=feature_request.md&title=
[repo-pull-requests]: https://github.com/prismicio-community/storybook-addon-gatsby/pulls

<!-- Badges -->

[npm-version-src]: https://img.shields.io/npm/v/storybook-addon-gatsby/latest.svg
[npm-version-href]: https://npmjs.com/package/storybook-addon-gatsby
[npm-downloads-src]: https://img.shields.io/npm/dm/storybook-addon-gatsby.svg
[npm-downloads-href]: https://npmjs.com/package/storybook-addon-gatsby
[github-actions-ci-src]: https://github.com/prismicio-community/storybook-addon-gatsby/workflows/ci/badge.svg
[github-actions-ci-href]: https://github.com/prismicio-community/storybook-addon-gatsby/actions?query=workflow%3Aci
[codecov-src]: https://img.shields.io/codecov/c/github/prismicio-community/storybook-addon-gatsby.svg
[codecov-href]: https://codecov.io/gh/prismicio-community/storybook-addon-gatsby
[conventional-commits-src]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg
[conventional-commits-href]: https://conventionalcommits.org
[license-src]: https://img.shields.io/npm/l/storybook-addon-gatsby.svg
[license-href]: https://npmjs.com/package/storybook-addon-gatsby
