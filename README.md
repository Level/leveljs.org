# leveldb.org

This is the source code for [leveldb.org](leveldb.org).

## CSS Structure
The CSS is located under `assets/css`, with the following architecture:

```
├── assets
  └── css
    ├── components
    ├── globals
    ├── sections
    ├── main.styl
    ├── normalize.css
    └── main.css
```

Where:

* **compontents** — are reusable components for common elements (such as buttons, forms, typography)
* **globals** — reusable variables, mixins and base for the website
* **pages** — pages of the website (comments, profile, 404, landing, etc.)
* **main.css** — main CSS stylesheet, importing other components
* **normalize.css** — browser resets

## Template Structure

```
├── assets
  └── templates
    ├── index.jade
    └── layout.jade
```

Where:

* **layout.jade** — basic layout file for the entire website
* **index.jade** — sample page (here being the landing page) that extends the layout

## How to run and compile
Feel free to use whatever tools that you are comfortable with. Example set up:

### To run in development mode, use:
```
npm start
```

### To run in production mode, use:
```
svccfg import ./service.xml
svcadm enable leveldb-org
```
