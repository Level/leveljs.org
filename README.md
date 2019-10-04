# leveljs.org

[![Backers on Open Collective](https://opencollective.com/level/backers/badge.svg?color=orange)](#backers)
[![Sponsors on Open Collective](https://opencollective.com/level/sponsors/badge.svg?color=orange)](#sponsors)

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
# hack on the codez, send pull request
```

### For maintainers

`npm run deploy` builds the static site, switches to the gh-pages branch and
puts the built site in the root, and then does git push origin gh-pages.

```
git fetch
git checkout master # if you're not already on it
git merge <fork-branch>
npm run deploy
```

## Donate

To sustain [`Level`](https://github.com/Level) and its activities, become a backer or sponsor on [Open Collective](https://opencollective.com/level). Your logo or avatar will be displayed on our 28+ [GitHub repositories](https://github.com/Level) and [npm](https://www.npmjs.com/) packages. 💖

### Backers

[![Open Collective backers](https://opencollective.com/level/backers.svg?width=890)](https://opencollective.com/level)

### Sponsors

[![Open Collective sponsors](https://opencollective.com/level/sponsors.svg?width=890)](https://opencollective.com/level)

## License

[MIT](LICENSE.md) © 2014-present Paolo Fragomeni and [Contributors](CONTRIBUTORS.md).
