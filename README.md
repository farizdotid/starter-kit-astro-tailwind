# Astro Starter Kit: Astro + Tailwind + Google Font Poppins

A lightweight, modern website template built with [Astro](https://astro.build) and [Tailwind CSS](https://tailwindcss.com).

## Features

- ⚡️ **Fast by default** - Leverages Astro's zero-JS-by-default approach
- 🎨 **Tailwind CSS** - Utility-first CSS framework for rapid styling
- 📱 **Responsive** - Looks great on all devices
- 🔍 **SEO-friendly** - Proper metadata and semantic structure
- 🚀 **Easy deployment** - Build and deploy to any static hosting
- 🧩 **Component-based** - Modular architecture for maintainability

## Quick Start

```bash
# Clone the repository
git clone https://github.com/farizdotid/starter-kit-astro-tailwind.git

# Navigate to the project
cd starter-kit-astro-tailwind

# Install dependencies
npm install

# Start the development server
npm run dev
```

Visit `http://localhost:3000` to see your site in action!

## Project Structure

```
├── public/              # Static assets
├── src/
│   ├── components/      # Reusable UI components
│   ├── layouts/         # Page layouts
│   ├── pages/           # Page templates (routes)
│   └── styles/          # Global styles
├── astro.config.mjs     # Astro configuration
├── tailwind.config.js   # Tailwind CSS configuration
└── package.json         # Project dependencies
```

## Customization

### Tailwind Configuration

Modify your Tailwind setup in `tailwind.config.js`:

```js
export default {
  content: ['./src/**/*.{astro,html,js,jsx,md,mdx,svelte,ts,tsx,vue}'],
  theme: {
    extend: {
      fontFamily: {
        poppins: ['Poppins', 'sans-serif'],
      },
    },
  },
  plugins: [],
}
```

### Creating New Pages

Add new pages to the `src/pages` directory:

```astro
---
// src/pages/contact.astro
import Layout from '../layouts/Layout.astro';
---

<Layout title="Contact | Astro Tailwind Starter">
  <main class="container mx-auto px-4 py-8">
    <h1 class="text-3xl font-bold">Contact Us</h1>
    <p>Your content here...</p>
  </main>
</Layout>
```

## Building for Production

```bash
# Build the production version
npm run build

# Preview the production build
npm run preview
```

Your optimized site will be in the `dist` directory, ready to be deployed.

## License

This template is MIT licensed. Feel free to use it for any project.

## Acknowledgements

- [Astro](https://astro.build)
- [Tailwind CSS](https://tailwindcss.com)