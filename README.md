# XelTemplates

Templates for bootstrapping a [Xel](https://github.com/dev-kas/Xel) project.

## 🚀 Usage

To scaffold a new Xel project:

```sh
xel init <template-name>
```

If no template is specified, it defaults to the one set in `~/.xel/config.json` under the `"defaultTemplate"` field. By default, this is set to `default`.

To manually pull a template from this repo:

```sh
xel templates pull https://github.com/dev-kas/XelTemplates/<template-name>
```

## 📦 Available Templates

* [`default`](./default): Basic starting point for any Xel project.

## 🤝 Contributing

Want to add your own template? Here's how:

1. Fork this repo.
2. Add your template as a new folder in the root (e.g. `/my-cool-template`).
3. Inside that folder, include:

   * A `xel.json` (with name, description, version, main file, etc.)
   * A `README.md` explaining how to use the template.
4. Keep your template versioned properly — see [Versioning Guide](#-versioning-guide) below.
5. Open a [Pull Request](https://github.com/dev-kas/XelTemplates/pulls).

To test your template locally before contributing:

```sh
xel templates pull <path-to-your-template>
```

## 📐 Versioning Guide

Templates follow [Semantic Versioning](https://semver.org/) with a template-specific interpretation:

* **MAJOR**: Structural or paradigm-breaking changes (e.g. switched from one framework/tooling style to another).
* **MINOR**: Non-breaking additions or improvements (e.g. added CI, docs, helpers).
* **PATCH**: Fixes, cleanup, or minor tweaks (e.g. typos, formatting, updated deps).

Each template manages its own version in its `xel.json`.
