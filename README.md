# select2-tailwindcss-theme

Links

[Select2](https://github.com/select2/select2) v4 theme for TailwindCSS v3.4

## Live demo

## 📦 Installation

1. Install the package:

Install the package and ensure you have TailwindCSS installed in your project:

```bash
# npm
$ npm install @erimicel/select-tailwindcss-theme

# yarn
$ yarn add @erimicel/select-tailwindcss-theme
```

## Usage

```bash
import 'select-tailwindcss-theme/dist/select2-tailwindcss-theme.css'; // Regular version
// OR
import 'tailwind-theme-extension/dist/select2-tailwindcss-theme.min.css'; // Minified version
```

```js
$('select').select2({
    theme: 'tailwindcss-3',
});
```

### With tailwindcss config

Update your Tailwind configuration to include the package in the content array:

```bash
// tailwind.config.js
module.exports = {
  content: [
    './src/**/*.{html,js}',
    './node_modules/tailwind-theme-extension/dist/*.css', // Include the package
  ],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

## Development

```bash
git clone https://github.com/erimicel/select2-tailwindcss-theme.git
cd select2-tailwindcss-theme
npm install
```

Modify the SCSS file in src/.scss. Build the CSS:

```bash
npm run build       # Regular CSS with @apply classes
npm run build:min   # Minified CSS
```

## Contributing

Contributions, issues, and feature requests are welcome! Fork the repository, create a new branch, commit your changes, push to your branch, and open a pull request:

```bash
git checkout -b feature-branch-name
git commit -m 'Add some feature'
git push origin feature-branch-name
```

If you find this package helpful, please ⭐ the repository on GitHub!