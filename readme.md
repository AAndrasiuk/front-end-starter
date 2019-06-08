# Front End Starter

Based on the [Webpack](https://webpack.js.org/) module bundler.

---

#### Used plugins and dependencies:

| Option                               | Description                                                                                               |
| ------------------------------------ | --------------------------------------------------------------------------------------------------------- |
| _terser-webpack-plugin_              | Minimize JS files                                                                                         |
| _optimize-css-assets-webpack-plugin_ | Minimize CSS files                                                                                        |
| _sass-loader_                        | Compiles SASS to CSS                                                                                      |
| _style-loader_                       | Instead of add `<style>` tag to `<head>` compiles CSS to separate CSS file                                |
| _html-webpack-plugin_                | Compiles a HTML file with atached scrits and styles                                                       |
| _babel_                              | Compiles ES5+ syntax into a backwards compatible version of JavaScript and creates polyfills if necessary |
| _webpack-dev-server_                 | Creates server with hot reloading                                                                         |
| _normalize.css_                      | Makes browsers render all elements more consistently and in line with modern standards                    |

---

#### Available Scripts

Create development build (files will not be compressed):

```js
npm run dev
```

Create production build (files will be compressed):

```js
npm run build
```

Develop with hot reloading:

```js
npm run start
```

---

#### Usage

Entry point for all files (scripts and styles) is `src/index.js`.

All the scripts imported into `index.js` will be compiled into one script `bundle.js`, styles will be compiled into `style.css`.

##### Import sass into sass files:

```css
@import "filename";
```

##### Import scripts and styles into index.js:

```js
import "filename";

import { component } from "./filename";

import component from "./filename";
```

##### Use jQuery:

```js
npm add jquery
```

Then import jQuery in any script file:

```js
import $ from "jquery";
```

![Preview](https://i.imgur.com/7fgoAKH.jpg "Main page")