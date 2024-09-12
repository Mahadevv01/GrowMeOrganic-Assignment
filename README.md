# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR (Hot Module Replacement) and includes some ESLint rules for better development practices.

# Project Name

This project is deployed and live at:

[react-assignment-two-blue.vercel.app](https://react-assignment-two-blue.vercel.app)


## Available Plugins

Currently, two official plugins are available for React in Vite:

- `@vitejs/plugin-react`: Uses Babel for Fast Refresh.
- `@vitejs/plugin-react-swc`: Uses SWC for Fast Refresh.

## Expanding the ESLint Configuration

If you are developing a production application, it is recommended to enhance the ESLint configuration by enabling type-aware lint rules.

### Update `parserOptions` in the ESLint Configuration:

Configure the top-level `parserOptions` property like this:

```json
{
  // other rules...
  "parserOptions": {
    "ecmaVersion": "latest",
    "sourceType": "module",
    "project": ["./tsconfig.json", "./tsconfig.node.json"],
    "tsconfigRootDir": "__dirname"
  }
}
