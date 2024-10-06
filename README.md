# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## GitHub pages

1. install `gh-pages`:

```bash
npm i gh-pages
```

2. Add to `package.json`:

```json
"scripts": {
  "deploy": "vite build && gh-pages -d dist"
}
```

3. Add base to `vite.config.js`:

```js
base: '/<REPO_NAME>/',
```

4. Deploy:

```bash
npm run deploy
```

5. Enable GitHub Pages in the repository settings.

6. Create token for GitHub Actions:
   Go to `Settings` -> `Developer settings` -> `Personal access tokens` -> `Generate new token`

- Contents: Read and Write

7. Add token to repository secrets
8. Add GitHub Actions workflow
