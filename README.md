# @du/eslint-config

> 🧠 Common ESLint configuration for TypeScript, React, and Prettier — used across all Du Nguyen projects.

## ✨ Features

- ✅ ESLint 9+ **Flat Config** compatible
- 🦾 TypeScript + React support out of the box
- 💅 Prettier integrated (no conflicting rules)
- 🔎 SonarJS for code smell detection
- ⚙️ Works in VSCode and CI/CD
- 🧩 Easily extendable for specific project needs

---

## 🚀 Installation

First, install this package **and its peer dependencies**:

```bash
npm install -D @du/eslint-config eslint prettier \
  @typescript-eslint/parser @typescript-eslint/eslint-plugin \
  eslint-plugin-react eslint-plugin-react-hooks \
  eslint-plugin-jsx-a11y eslint-plugin-sonarjs \
  eslint-config-prettier
```

or with Yarn:

```bash
yarn add -D @du/eslint-config eslint prettier \
  @typescript-eslint/parser @typescript-eslint/eslint-plugin \
  eslint-plugin-react eslint-plugin-react-hooks \
  eslint-plugin-jsx-a11y eslint-plugin-sonarjs \
  eslint-config-prettier
```

🧩 Usage (ESLint 9+ Flat Config)

Create a file called eslint.config.js in your project root:

⚛️ React Projects

This config automatically supports React (.jsx, .tsx),
but you can also import React-specific rules only:

```bash
import reactConfig from "@du/eslint-config/rules/react.js";

export default [...reactConfig];
```
