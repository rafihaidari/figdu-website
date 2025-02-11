Here’s the completed and polished `README.md` for **FigDU** based on your provided content:

---

<p align="center">
  <img src="/static/img/FigDu-Logo.png" alt="FigDU Logo" width="80px">
</p>

<h1 align="center">FigDU - Figma Developer Utility</h1>

<p align="center">
  <a href="https://app.fossa.com/projects/git%2Bgithub.com%2Frafihaidari%2Ffigdu?ref=badge_small" target="_blank">
    <img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Frafihaidari%2Ffigdu.svg?type=small" alt="FOSSA Status">
  </a>
  <a href="https://app.fossa.com/projects/git%2Bgithub.com%2Frafihaidari%2Ffigdu?ref=badge_shield&issueType=security" target="_blank">
    <img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Frafihaidari%2Ffigdu.svg?type=shield&issueType=security" alt="FOSSA Status">
  </a>
</p>

<p align="center">
  <strong>Your all-in-one toolkit for creating powerful Figma plugins.</strong>
</p>

<p align="center">
  FigDU is made by developers, for developers. Build your Figma plugins with ease and stop worrying about configuration files and the odd peculiarities of building for Figma. With FigDU, you can focus on creating amazing plugins while we handle the boilerplate, build process, and tooling.
</p>

---

## 🌟 Features

- **Zero-config setup**: Start building your Figma plugin immediately without worrying about configuration files.
- **Built-in React support**: Build your plugin UI with React, the most popular front-end library.
- **Chakra UI integration**: Create beautiful, responsive UIs with Chakra UI's pre-built components.
- **Hot Reload**: See your changes in real-time as you develop your plugin.
- **Figma API Helpers**: Pre-configured utilities to interact with the Figma API seamlessly.
- **Plugin Manifest Generator**: Automatically generate the `manifest.json` file for your plugin.
- **Optimized Build Process**: Production-ready builds with minification and bundling.

---

## 🚀 Quick Start

To create a new FigDU project, run the following command:

```bash
npx create-figdu
```

or

```bash
npm create figdu
```

This will set up a new FigDU project in your current directory with all the necessary files and configurations.

---

## 🛠️ Getting Started

1. **Create a new project**:

   ```bash
   npx create-figdu
   ```

2. **Navigate to your project directory**:

   ```bash
   cd your-figdu-project
   ```

3. **Build your project**:

   - For a one-time build, run:
     ```bash
     npm run build
     ```
   - To watch for changes and rebuild automatically, run:
     ```bash
     npm run watch
     ```

4. **Open Figma**:

   - Go to the **Plugins** menu in Figma.
   - Select **Development** > **Import plugin from manifest**.
   - Choose the `manifest.json` file in your project directory.

5. **Start coding**:
   - Edit the `src` folder to build your plugin.
   - Use React and Chakra UI to create stunning plugin UIs.
   - FigDU will automatically reload your plugin as you make changes.

---

## 🏗️ Building for Production

When you're ready to ship your plugin, run:

```bash
npm run build
```

This will generate an optimized production build in the `dist` folder. You can then package and publish your plugin to the Figma Plugin Store.

---

## 🧩 Why React and Chakra UI?

- **React**: A powerful and flexible library for building user interfaces. With React, you can create reusable components and manage state efficiently.
- **Chakra UI**: A simple, modular, and accessible component library that provides pre-built, customizable components to speed up your development process.

Together, React and Chakra UI make it easy to build beautiful, responsive, and maintainable UIs for your Figma plugins.

---

## 📂 Repository & Website

- **GitHub Repository**: [https://github.com/rafihaidari/figdu](https://github.com/rafihaidari/figdu)
- **Website**: [https://figdu.com](https://figdu.com)

---

## 🤝 Contributing

We welcome contributions! If you'd like to improve FigDU, please drop an email: **hello.rafihaidari@gmail.com**.

---

## 📄 License

FigDU is open-source and licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Frafihaidari%2Ffigdu.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Frafihaidari%2Ffigdu?ref=badge_large)

---

## 🙏 Acknowledgments

- Built with ❤️ in Germany.

---

Happy plugin building! 🚀