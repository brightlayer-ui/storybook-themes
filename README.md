# Brightlayer UI themes for Storybook applications
[![](https://img.shields.io/circleci/project/github/brightlayer-ui/storybook-themes/master.svg?style=flat)](https://circleci.com/gh/brightlayer-ui/storybook-themes/tree/master)
[![](https://img.shields.io/npm/v/@brightlayer-ui/storybook-themes.svg?label=@brightlayer-ui/storybook-themes&style=flat)](https://www.npmjs.com/package/@brightlayer-ui/storybook-themes)

This package contains theming support for [Storybook](https://storybook.js.org/) applications built using Angular or React. It is primarily used to give these applications a Brightlayer UI look and feel. Integrating this theme into your storybook application will change the appearance of the storybook container and any Markdown notes found within the `@storybook/addon-notes` add-on.

## Installation

This theme package depends on [@brightlayer-ui/colors](https://www.npmjs.com/package/@brightlayer-ui/colors) and the [@storybook/theming](https://www.npmjs.com/package/@storybook/theming) add-on. To begin, install all three by running:

```
yarn add @brightlayer-ui/colors @storybook/theming @brightlayer-ui/storybook-themes
```

## Usage

To integrate the theme into your storybook app, add the following code to your config:

```typescript
import { bluiTheme } from '@brightlayer-ui/storybook-themes';
import { addParameters } from '@storybook/react';

addParameters({
    options: {
        theme: bluiTheme,
    },
});
```

For additional help while integrating storybook themes, see the [storybook docs](https://storybook.js.org/docs/configurations/theming/).

## Demos

You can see this theme in action in the documentation for Brightlayer UI component libraries at [brightlayer-ui-components.github.io](https://brightlayer-ui-components.github.io).
