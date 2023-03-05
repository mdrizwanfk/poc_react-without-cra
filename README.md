# POC: React App built without CRA (Create React App)

Create React App is a Reactjs Build-Tool/toolchain.

For more info, read from [here](https://create-react-app.dev/).

---

Installed packages:
Dependencies:

- react, react-dom: react libraries.

Dev Dependencies:

- webpack, webpack-cli, webpack-dev-server: bundling web assets, easy cli commands to setup a webpack app, dev-server to bundle up with fresh changes and serve them for local development. more detailed info here, [[webpack]]

- @babel/core: core transpiler, for more info about babel and how is it different from webpack (- in short, babel is a compiler, webpack is a module bundler), check here, [[babel]].

- babel-loader(js files), style-loader(css files, adds styles to dom using style tags), sass-loader(scss files, converts sass to css): loaders are used by webpack that dictate rules to preprocess file-types as they are loaded/imported when bundling, like js, jsx, scss, etc.. to a normal, browser-understandable format.

- @babel/preset-react: `preset-react` is a Babel preset that includes plugins for React syntax and features⁵. For example, it enables JSX transformation, React automatic runtime, development mode helpers, etc⁵.

Some other tools also use `preset-react` as a name for their own presets that configure React projects. For example, Nx has a `react-standalone` preset that sets up a React application with testing and linting². Storybook has a `preset-create-react-app` that configures Storybook to work with Create React App³¹. Neutrino has a `@neutrinojs/react` preset that builds modern React web applications with zero upfront configuration⁴.

Source: Conversation with Bing, 05/03/2023(1) @babel/preset-react · Babel. https://babeljs.io/docs/babel-preset-react Accessed 05/03/2023.
(2) Create a Preset | Nx. https://nx.dev/recipes/advanced-plugins/create-preset Accessed 05/03/2023.
(3) Storybook Tutorials - js. https://storybook.js.org/tutorials/create-an-addon/react/en/preset/ Accessed 05/03/2023.
(4) Storybook Tutorials - js. https://storybook.js.org/tutorials/create-an-addon/react/en/preset/ Accessed 05/03/2023.
(5) React - Neutrino. https://neutrinojs.org/packages/react/ Accessed 05/03/2023.
(6) @umijs/preset-react - npm. https://www.npmjs.com/package/@umijs/preset-react Accessed 05/03/2023.

- @babel/preset-env: `preset-env` is a Babel preset that allows you to use the latest JavaScript features without worrying about which syntax transforms and polyfills are needed for your target environments¹². You can specify your targets using browserslist queries or a configuration file¹³.

There is also a PostCSS Preset Env that does something similar for CSS features. It lets you use modern CSS syntax and features with automatic polyfills and fallbacks⁵.

Source: Conversation with Bing, 05/03/2023(1) @babel/preset-env · Babel. https://babeljs.io/docs/babel-preset-env Accessed 05/03/2023.
(2) How babel preset-env, core-js, and browserslistrc work together. https://www.valentinog.com/blog/preset-env/ Accessed 05/03/2023.
(3) What you don’t know about BabelJS preset-env | PerimeterX. https://www.perimeterx.com/tech-blog/2022/what-you-don-t-know-about-babeljs-preset-env/ Accessed 05/03/2023.
(4) PostCSS Preset Env - CSSTools. https://preset-env.cssdb.org/ Accessed 05/03/2023.
(5) @babel/preset-env - npm. https://www.npmjs.com/package/@babel/preset-env Accessed 05/03/2023.

- html-webpack-plugin - HtmlWebpackPlugin is a webpack plugin that simplifies creation of HTML files to serve your webpack bundles¹. It can generate an HTML file for you, or use your own template¹. It is useful for webpack bundles that include a hash in the filename which changes every compilation¹³.
	- To use HtmlWebpackPlugin, you need to install it first by running `npm i html-webpack-plugin`⁶ or `yarn add --dev html-webpack-plugin`⁵. Then, you need to add the plugin to your webpack configuration file¹⁵. You can either let the plugin generate an HTML file for you, or use a custom template by assigning the `template` property with the template file path³⁴.

Do you have any questions about HtmlWebpackPlugin?

Source: Conversation with Bing, 05/03/2023(1) html-webpack-plugin - npm. https://www.npmjs.com/package/html-webpack-plugin Accessed 05/03/2023.
(2) HtmlWebpackPlugin | webpack. https://webpack.js.org/plugins/html-webpack-plugin/ Accessed 05/03/2023.
(3) How to Setup Html Webpack Plugin | Rapid Develop. https://rapidevelop.org/webpack/setup-html-webpack-plugin Accessed 05/03/2023.
(4) GitHub - jantimon/html-webpack-plugin: Simplifies creation of HTML .... https://github.com/jantimon/html-webpack-plugin Accessed 05/03/2023.
(5) How to use Webpack and HTML Webpack Plugin | Simple Guide. https://www.strobecorp.com/html-webpack-plugin/ Accessed 05/03/2023.
(6) How to Setup HTML Webpack Plugin - Communicode. https://communicode.io/how-to-setup-html-webpack-plugin/ Accessed 05/03/2023.