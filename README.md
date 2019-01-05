# leveldb.org

This is the source code for [leveldb.org](http://leveldb.org).

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

* **compontents** — are reusable components for common elements (such as buttons, forms, typography)
* **globals** — reusable variables, mixins and base for the website
* **pages** — subpages of the website (comments, profile, 404, landing, etc.)
* **sections** - individual sections of a page (header, footer, community, platforms, etc.)

## Template Structure

```
├── assets
  └── templates
    ├── index.jade
    ├── footer.jade
    └── layout.jade
```

Where:

* **layout.jade** — basic layout file for the entire website
* **index.jade** — the page content (here being the landing page)
* **footer.jade** - footnotes

## Contributing

[`Level/leveldb.org`](https://github.com/Level/leveldb.org) is an **OPEN Open Source Project**. This means that:

> Individuals making significant and valuable contributions are given commit-access to the project to contribute as they see fit. This project is more like an open wiki than a standard guarded open source project.

See the [Contribution Guide](https://github.com/Level/community/blob/master/CONTRIBUTING.md) for more details.

### For contributors
```
git clone https://github.com/Level/leveldb.org.git
cd leveldb.org
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

### To run in production mode on a SmartOS server, use:
```
svccfg import ./service.xml
svcadm enable leveldb-org
```

## License

[MIT](LICENSE.md) © 2014-present Paolo Fragomeni and [Contributors](CONTRIBUTORS.md).
