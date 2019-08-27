# React External Link

[![Paypal Donate](https://img.shields.io/badge/Donate-paypal-blue.svg?style=flat-square&logo=paypal&colorA=cccccc)](https://acel.me/donate)

This library provides a simple `ExternalLink` component for [react](https://es.reactjs.org/) which can be used to render `a` tags with both `target="_blank"` and `rel="noopener noreferrer"` attributes.

## Installation

Using npm: `npm istall react-external-link --save`

Using yarn: `yarn add react-external-link`

## Usage

If you just need a simple link with no custom text:

```tsx
import React from 'react';
import { ExternalLink } from 'react-external-link';

const MyComponent = () => (
  <div>
    <ExternalLink href="https://example.com" />
  </div>
);

export default MyComponent;
```

This will be rendered as `<a href="https://example.com" target="_blank" rel="noopener noreferrer">https://example.com</a>`.

If you need to provide a custom content, you can do so by providing the `ExternalLink`'s `children`:

```tsx
import React from 'react';
import { ExternalLink } from 'react-external-link';

const MyComponent = () => (
  <div>
    <ExternalLink href="https://example.com">
      <span>Visit the site</span>
    <ExternalLink>
  </div>
);

export default MyComponent;
```

This will be rendered as:

```html
<a href="https://example.com" target="_blank" rel="noopener noreferrer">
  <span>Visit the site</span>
</a>
```
