# Elegant Portfolio Template

> Live version of markdown [here](https://github.com/fran-gzz/portfolio-template-readme).

> 🧑‍🚀 **Live preview?** [Here!](https://portfolio-template-neon.vercel.app/)


![preview-image](https://fran-gzz.github.io/portfolio-template-readme/assets/preview.png)


This is a modern and responsive portfolio template for developers and designers. Perfect for showcasing projects, skills, and work experience.

### Requeriments
- Node.js
- Astro
- Tailwind CSS

### Installation
1. Install dependencies: `npm install`
2. Start the development server: `npm run dev`

### Configuration
Elements like name, projects, and skills can be configured in the `cv.json` file on the root. Ensure you follow the existing structure.

### Customization
- **Images:** Portfolio images are located in the `public` folder. Replace these images with your own. I recommend using the `webp` format for images


### Project Structure

Inside the project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
│   └── me.webp
├── src/
│   ├── components/
│   │   └── BaseHead.astro
│   │   └── Button.astro
│   │   └── Section.astro
│   │   └── ui/About.astro
│   │   └── ui/Hero.astro
│   │   └── ui/Projects.astro
│   │   └── ui/Skills.astro
│   │   └── ui/Work.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── project/[...slug].astro
│       └── index.astro
├── cv.json <-- EDIT WITH YOUR DATA HERE
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

### Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

### License
This project is under the regular Envato license (or extended as applicable). See `LICENSE.md` for more details.