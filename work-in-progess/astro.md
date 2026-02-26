# 🚀 ASTRO - CHEAT SHEET

## 🛠 1. INSTALLATION & SETUP

### Créer un nouveau projet
pas de install -g ou autre juste cette commande 
``` bash
npm create astro@latest 
```


### Intégrations courantes
```bash
npx astro add tailwind      # CSS Utility-first
npx astro add react         # Composants React
npx astro add sitemap       # Génération de sitemap SEO
npx astro add mdx           # Support Markdown étendu
```

### Commandes CLI
- `npm run dev`     : Lancer le serveur local (http://localhost:4321)
- `npm run build`   : Générer le build statique dans /dist
- `npm run preview` : Tester le build localement avant déploiement

---

## 🏗 2. STRUCTURE D'UN COMPOSANT (.astro)
```js
---
// --- PARTIE SCRIPT (JavaScript/TypeScript) ---
import MyComponent from '../components/MyComponent.astro';
const { title = "Valeur par défaut" } = Astro.props;
const items = ["A", "B", "C"];

---


<header>
  <h1>{title}</h1>
</header>

<ul>
  {items.map((item) => <li>{item}</li>)}
</ul>

<slot /> 

<style>
  h1 { color: #333; }
</style>
```
---


## 📂 3. ROUTAGE & PAGES
- src/pages/index.astro       => /
- src/pages/about.astro       => /about
- src/pages/projects/[id].astro => Route dynamique

---

## 📁 4. CONTENT COLLECTIONS (Gestion de données)

**Configuration : src/content/config.ts**
```js
import { z, defineCollection } from 'astro:content';
const projects = defineCollection({
  type: 'content',
  schema: z.object({
    title: z.string(),
    description: z.string(),
    pubDate: z.date(),
    tags: z.array(z.string()),
  }),
});
export const collections = { projects };
```
---

## 🏝 5. CLIENT DIRECTIVES (Hydratation JS)
- <Component client:load />    : Charge immédiatement.
- <Component client:idle />    : Charge quand le navigateur est au repos.
- <Component client:visible /> : Charge quand l'élément apparaît à l'écran.

---

## 🖼 6. ASSETS & IMAGES
import { Image } from 'astro:assets';
import monImageLocal from '../assets/photo.png';
```js
<Image src={monImageLocal} alt="Description" width={600} />
```
---

## ⚙️ 7. CONFIGURATION GITHUB PAGES (astro.config.mjs)
```
import { defineConfig } from 'astro/config';
import tailwind from '@astrojs/tailwind';

export default defineConfig({
  site: '[https://ton-pseudo.github.io](https://ton-pseudo.github.io)',
  base: '/nom-du-repo', 
  integrations: [tailwind()],
  output: 'static',
});
```