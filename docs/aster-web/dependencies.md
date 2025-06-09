---
title: Dependencies
layout: default
has_toc: false
parent: Aster Web
nav_order: 99
---

# Dependencies for Aster Web
This page lists the dependencies the [Aster Web] project and their purposes where necessary.

- [Svelte](https://svelte.dev/) - Javascript Framework
- [Vite](https://vite.dev/) - Build Tool
- [Typescript](https://www.typescriptlang.org/)
- [svelte-awesome-color-picker](https://github.com/Ennoriel/svelte-awesome-color-picker) - A colour picker for use in theme options.
- [marked](https://marked.js.org/) - Primary markdown parser used for messages.
- [snarkdown](https://www.npmjs.com/package/snarkdown/v/1.0.2) - A lightweight markdown parser used for the changelog.
- [svelte-i18n](https://www.npmjs.com/package/@jill64/svelte-i18n) - Used for localisation.
- [svelte-icons-pack](https://www.npmjs.com/package/svelte-icons-pack) - Used for easy access to graphic icons.
- [svelte-markdown](https://www.npmjs.com/package/svelte-markdown) - Svelte based implementation of the [marked] package.
- [svelte-media-queries](https://www.npmjs.com/package/svelte-media-queries) - Used for responsive web design within the app.

## Full Package File
The full dependencies sections of the `package.json` file for [Aster Web]. Last updated for version α-2.4.0.

```json
  "devDependencies": {
    "@sveltejs/vite-plugin-svelte": "^3.1.1",
    "@tsconfig/svelte": "^5.0.4",
    "svelte": "^4.2.18",
    "svelte-awesome-color-picker": "^3.1.0",
    "svelte-check": "^3.8.1",
    "tslib": "^2.6.3",
    "typescript": "^5.2.2",
    "vite": "^5.3.1"
  },
  "dependencies": {
    "marked": "^15.0.12",
    "snarkdown": "^2.0.0",
    "svelte-i18n": "^4.0.1",
    "svelte-icons-pack": "^3.1.3",
    "svelte-markdown": "^0.4.1",
    "svelte-media-queries": "^1.6.2"
  }
```

---
[Aster Web]: ../index.md