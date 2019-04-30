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
