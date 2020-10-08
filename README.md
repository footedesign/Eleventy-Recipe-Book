# Eleventy Recipe Book

Eleventy Recipe Book is for quickly setting up a simple digital recipe book. Built on top of [Eleventy Starter Boilerplate](https://github.com/ixartz/Eleventy-Starter-Boilerplate) utilizing [Eleventy](https://www.11ty.dev).

Clone this project and use it to create your own [Eleventy](https://www.11ty.dev) Recipe Book. You can view the demo [here](https://footedesign.github.io/Eleventy-Recipe-Book).

### Inspiration

- A clean and minimal way to utilize your own/adapted recipes
- [Wilto Makes Food](https://wiltomakesfood.com/)
- [OpenEats](https://github.com/open-eats/OpenEats)

### Core Features

A clean and minimal digital recipe book built on top of [Eleventy Starter Boilerplate](https://github.com/ixartz/Eleventy-Starter-Boilerplate) including:
- [11ty](https://www.11ty.dev) for site generation
- Lazy load images with [lazysizes](https://github.com/aFarkas/lazysizes)
- Image compression with [Imagemin](https://github.com/imagemin/imagemin)
- Minified HTML & CSS with [HTMLMinifier](https://www.npmjs.com/package/html-minifier) and [cssnano](https://cssnano.co)
- Module Bundling with [Webpack](https://webpack.js.org)
- Sitemap.xml
- 404 page
- Pagination
- Cache busting
- [And more](https://github.com/ixartz/Eleventy-Starter-Boilerplate)

### Requirements

- Node.js and npm

### Getting Started

Run the following command in your local environment:

```
git clone --depth=1 https://github.com/footedesign/Eleventy-Recipe-Book.git my-project-name
cd my-project-name
npm install
```

Then, you can run locally in development mode with live reload:

```
npm run dev
```

Open http://localhost:8080 with your favorite browser to see your digital recipe book.

### Project structure

```
.
├── public              # Static files
│   └── assets
│       └── images      # Images not needed by Webpack
└── src
    ├── _data           # Eleventy data folder
    ├── _includes
    │   └── layouts     # HTML layout files
    ├── assets          # Assets folder that needs to be processed by Webpack
    │   ├── images
    │   │   └── recipes # Images used in your recipes (will be compressed by Webpack)
    │   └── styles      # Your site CSS files
    └── recipes         # Your recipes
```

### Customization

You can easily configure your Eleventy Recipe Book by changing the following files:

- `public/assets/images/logo.png`: your site logo
- `public/apple-touch-icon.png`, `public/favicon.ico`, `public/favicon-16x16.png` and `public/favicon-32x32.png`: your site favicon, you can generate one at https://favicon.io/favicon-generator/
- `src/_data/site.json`: your site configuration
- `src/_includes/layouts`: your site HTML layout
- `src/assets/styles/main.css`: your site CSS file using Tailwind CSS

### Deploy to production

You can see the results locally in production mode with:

```
npm run serve
```

The generated HTML and CSS files are minified. Unused CSS will also be removed from [Tailwind CSS](https://tailwindcss.com).

You can create an optimized production build with:

```
npm run build
```

Now, your recipe book is ready to be deployed. All generated files are located in the `_site` folder, which you can deploy with any hosting service.

### Deploy to Netlify

Clone this repository to your own GitHub account and deploy to Netlify:

[![Netlify Deploy button](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/footedesign/Eleventy-Recipe-Book)

### Future Work

* [ ] improve recipe instruction readability
* [ ] rethink Eleventy tagging for grouping recipe types
* [ ] localStorage shopping list
* [ ] utilize a logo?
* [ ] [Extract Components](https://tailwindcss.com/docs/extracting-components) from Tailwind CSS
* [ ] Cooking mode: recipe instructions in easily digestable chunks for use during cooking
* [ ] Netlify CMS

### Contributions

Contributions are welcome. Feel free to open an issue if you have question or found a bug.

### License

Licensed under the MIT License, Copyright © 2020

See [LICENSE](LICENSE) for more information.