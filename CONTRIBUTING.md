# Contributing to SwissJS

We're excited that you're interested in contributing to the SwissJS platform website!

## Ways to Contribute

1.  **Bug Reports**: If you find an issue with the website or documentation, please report it via [GitHub Issues](https://github.com/kibologic/swissjs-website/issues).
2.  **Feature Suggestions**: Have an idea for a new feature or improvement? Start a discussion in [GitHub Discussions](https://github.com/kibologic/swissjs-website/discussions).
3.  **Pull Requests**: We welcome code contributions! Please ensure your PRs follow the style and architecture of the existing codebase.

## Development Style

- **Framework First**: All UI should be built using SwissJS components.
- **Systematic Styling**: Use the defined CSS variables and utility grids for consistency.
- **Mobile First**: All sections must be fully responsive and tested across different viewport sizes.
- **High Performance**: Avoid unnecessary re-renders and keep component state localized.

## Technical Requirements

- All code must pass current SwissJS compilation standards.
- Ensure all new components are tested for both **Light** and **Dark** mode compatibility.

## Package Names

The correct public package names for SwissJS are `@swissjs/core`, `@swissjs/router`, `@swissjs/compiler`, etc. All documentation and code examples shown to users must use the `@swissjs/` namespace.

Note: the site's own source files import from `@kibologic/core` for legacy build compatibility — this is intentional and should not be changed. However, any new documentation content, code snippets, or references visible to end users must always use the `@swissjs/` package prefix.
