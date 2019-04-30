# sveltejs-template-typescript
Quick and dirty demo of how simple it is to get TS working with the [vanilla Svelte 3 template](https://github.com/sveltejs/template).

Based on [this revision](https://github.com/sveltejs/template/tree/acfae9afc92e088062923199f81cf99ad145f310).

## Change Summary

- Add TypeScript devDependencies:
    - `typescript`
    - `tslib`
    - `rollup-plugin-typescript`
- Add new files:
    - `tsconfig.json`
    - `src/@types/svelte.d.ts`
- Rename `src/main.js` to `src/main.ts`
- Update `rollup.config.js`:
    - Change reference to `src/main.js` -> `src/main.ts`
    - Import and insert `typescript()` before `svelte()` in list

*Psst — looking for a shareable component template? Go here --> [sveltejs/component-template](https://github.com/sveltejs/component-template)*

---

# svelte app

This is a project template for [Svelte](https://svelte.technology) apps. It lives at https://github.com/sveltejs/template.

To create a new project based on this template using [degit](https://github.com/Rich-Harris/degit):

```bash
npx degit sveltejs/template svelte-app
cd svelte-app
```

*Note that you will need to have [Node.js](https://nodejs.org) installed.*


## Get started

Install the dependencies...

```bash
cd svelte-app
npm install
```

...then start [Rollup](https://rollupjs.org):

```bash
npm run dev
```

Navigate to [localhost:5000](http://localhost:5000). You should see your app running. Edit a component file in `src`, save it, and reload the page to see your changes.


## Deploying to the web

### With [now](https://zeit.co/now)

Install `now` if you haven't already:

```bash
npm install -g now
```

Then, from within your project folder:

```bash
now
```

As an alternative, use the [Now desktop client](https://zeit.co/download) and simply drag the unzipped project folder to the taskbar icon.

### With [surge](https://surge.sh/)

Install `surge` if you haven't already:

```bash
npm install -g surge
```

Then, from within your project folder:

```bash
npm run build
surge public
```
