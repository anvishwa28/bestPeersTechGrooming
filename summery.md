#  Vite vs Create React App  

##  Core Architecture
- **Vite**: Native ESM, esbuild, Rollup, fast HMR
- **CRA**: Webpack (dev/prod), abstracted config, slower rebuilds

##  Performance
- **Vite**: Instant dev start, fast HMR, efficient builds
- **CRA**: Slower start, full reloads, larger project impact

##  Configuration
- **Vite**: Accessible `vite.config.js`, Rollup plugins
- **CRA**: Hidden configs, needs CRACO/react-app-rewired for changes

##  React Support
- **Vite**: Fast Refresh, flexible but less React opinionated
- **CRA**: React-first, built-in testing/linting, PWA support

## Migration Notes
- Env vars: `import.meta.env` (Vite) vs `process.env` (CRA)
- Move test config, update imports, asset/public path tweaks
- Convert Jest to Vitest if needed

## Advanced Features
- **CSS**: Vite = fast HMR, CRA = Sass/PostCSS included
- **Testing**: CRA = Jest built-in, Vite = Vitest (separate setup)
- **TypeScript**: Vite = faster via esbuild, CRA = integrated

## Production & Deployment
- **Vite**: Modern output, better subdir/base support
- **CRA**: Stable with React-first platforms

## Tool Recommendation
Choose **Vite** if:
- You value speed, flexibility, multi-framework support

Choose **CRA** if:
- You want React-specific tooling, stability, and community support
