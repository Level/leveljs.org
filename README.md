# leveldb.org

This is the source code for [leveldb.org](leveldb.org).

## Stylus Structure
The Stylus files are located under `assets/static/styl`, with the following architecture...

```
├── assets
  └── styl
    ├── components
    ├── globals
    ├── pages
    └── main.styl
```

Where:

* **compontents** — are reusable components for common elements (such as buttons, forms, typography)
* **globals** — reusable variables, mixins and base for the website
* **pages** — pages of the website (comments, profile, 404, landing, etc.)

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

## Contributing

### For contributors
```
git clone https://github.com/Level/leveldb.org.git
cd leveldb.org
npm i
npm start
# hack on the codez, send pull request
```

### For maintainers
```
git pull <fork-branch>
# make sure changes look good
npm run deploy
```

`npm run deploy` builds the static site, switches to the gh-pages branch and 
puts the built site in the root, and then does git push origin gh-pages.

### To run in production mode on a SmartOS server, use:
```
svccfg import ./service.xml
svcadm enable leveldb-org
```
