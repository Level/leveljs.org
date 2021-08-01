# leveljs.org

This is the source code for [leveljs.org](http://leveljs.org).

## Stylus Structure

The Stylus files are located under `assets/static/styl`, with the following architecture...

```
├── assets
  └── styl
    ├── components
    ├── globals
    ├── pages
    ├── sections
    └── main.styl
```

Where:

- **compontents** — are reusable components for common elements (such as buttons, forms, typography)
- **globals** — reusable variables, mixins and base for the website
- **pages** — subpages of the website (comments, profile, 404, landing, etc.)
- **sections** - individual sections of a page (header, footer, community, platforms, etc.)

## Template Structure

```
├── assets
  └── templates
    ├── index.pug
    ├── footer.pug
    └── layout.pug
```

Where:

- **layout.pug** — basic layout file for the entire website
- **index.pug** — the page content (here being the landing page)
- **footer.pug** - footnotes

## Contributing

[`Level/leveljs.org`](https://github.com/Level/leveljs.org) is an **OPEN Open Source Project**. This means that:

> Individuals making significant and valuable contributions are given commit-access to the project to contribute as they see fit. This project is more like an open wiki than a standard guarded open source project.

See the [Contribution Guide](https://github.com/Level/community/blob/master/CONTRIBUTING.md) for more details.

### For contributors

```
git clone https://github.com/Level/leveljs.org.git
cd leveljs.org
npm i
npm start
```

### For maintainers

Manually trigger the GitHub Actions workflow to deploy to gh-pages.

## Donate

Support us with a monthly donation on [Open Collective](https://opencollective.com/level) and help us continue our work.

## License

[MIT](LICENSE)
