---
sidebar_position: 1
---

# Introduction to FigDU

**FigDU** is your **all-in-one toolkit for creating powerful Figma plugins**, made by developers for developers. It simplifies plugin development by handling the boilerplate, build process, and tooling, allowing you to focus on creating amazing plugins.

## Getting Started

### What you'll need

- [Node.js](https://nodejs.org/en/download/) version 18.0 or above:
  - When installing Node.js, check all checkboxes related to dependencies.

## Install FigDU

To create a new FigDU project, run the following command:

```bash
npx create-figdu
```

or

```bash
npm create figdu
```

This will set up a new FigDU project in your current directory with all necessary files and configurations.

## Start your Project

Navigate into your project directory:

```bash
cd your-figdu-project
```

Run the development server:

```bash
npm run dev
```

This command starts a local development environment, allowing you to build your plugin interactively.

## Features of FigDU

- **Zero-config setup**: Start building immediately without configuration hassles.
- **Built-in React support**: Leverage React for plugin UI development.
- **Chakra UI integration**: Use pre-built components for beautiful, responsive UIs.
- **Hot Reload**: See real-time changes while developing your plugin.
- **Figma API Helpers**: Utilities to simplify Figma API interactions.
- **Plugin Manifest Generator**: Automatically generates the `manifest.json` file.
- **Optimized Build Process**: Ensures production-ready builds with minification and bundling.

## Build for Production

When you're ready to deploy your plugin, run:

```bash
npm run build
```

This command generates an optimized build in the `dist` folder, ready for packaging and publishing to the Figma Plugin Store.