# 🎨 Vue 3 + Vite Starter

A modern Vue 3 template with Vite, TypeScript, and Docker support to help you get started quickly with professional development practices.

---

## 🛠️ Tech Stack

| Technology        | Details                                   |
| ----------------- | ----------------------------------------- |
| 🖖 **Vue**        | Vue 3 with Composition API                |
| ⚡ **Vite**       | Next-generation frontend tooling (v7.3.0) |
| 📘 **TypeScript** | Full type safety for JavaScript           |
| 🐳 **Docker**     | Containerized development & production    |
| 🎯 **ESLint**     | Code quality and consistency              |

---

## 📋 Prerequisites

- **Node.js** 16.x or higher
- **npm** or **pnpm** (recommended)
- **Docker** & **Docker Compose** (for containerized development)

---

## 🚀 Quick Start

### Local Development

#### Install Dependencies

```sh
npm install
```

#### Start Dev Server

Compile with hot-reload for development:

```sh
npm run dev
```

#### Build for Production

Type-check, compile, and minify:

```sh
npm run build
```

#### Lint Code

Check code quality with ESLint:

```sh
npm run lint
```

---

## 🐳 Docker Setup

### Development with Docker

Build and start the development container:

```sh
docker-compose -f docker-compose.yml up --build
```

The application will be available at `http://localhost:5173`

### Development with Hot Reload (Dockerfile.dev)

For faster development with automatic reloading:

```sh
docker-compose -f docker-compose.yml -f Dockerfile.dev up --build
```

### Production Build

Build the production image:

```sh
docker build -f Dockerfile -t vuebasics:latest .
```

Run production container:

```sh
docker run -p 5173:5173 vuebasics:latest
```

### Stop Containers

```sh
docker-compose down
```

---

## 💻 Recommended IDE Setup

**VS Code** + **Vue (Official)** Extension

- Install [Vue.js Official Extension](https://marketplace.visualstudio.com/items?itemName=Vue.volar)
- Disable Vetur extension if installed
- Enable [Turn on Custom Object Formatter](http://bit.ly/object-formatters)

---

## 🌐 Recommended Browser Setup

### Chromium-based (Chrome, Edge, Brave)

- Install [Vue.js DevTools](https://chromewebstore.google.com/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd)
- Enable [Custom Object Formatter in Chrome DevTools](http://bit.ly/object-formatters)

### Firefox

- Install [Vue.js DevTools](https://addons.mozilla.org/en-US/firefox/addon/vue-js-devtools/)
- Enable [Custom Object Formatter in Firefox](https://fxdx.dev/firefox-devtools-custom-object-formatters/)

---

## 📘 TypeScript Support

TypeScript cannot handle `.vue` file types by default. This project uses:

- **`vue-tsc`** - Replaces `tsc` CLI for type checking
- **[Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar)** - Makes VS Code aware of `.vue` types

---

## ⚙️ Configuration

- **Vite Configuration**: See [Vite Configuration Reference](https://vite.dev/config/)
- **TypeScript Config**: `tsconfig.json`
- **ESLint Config**: `eslint.config.ts`

---

## 📁 Project Structure

```
src/
├── components/       # Reusable Vue components
├── router/          # Vue Router configuration
├── stores/          # Pinia state management
├── views/           # Page components
├── assets/          # Styles and static assets
└── main.ts          # Application entry point
```

---

## 📝 Available Scripts

| Command         | Description              |
| --------------- | ------------------------ |
| `npm run dev`   | Start development server |
| `npm run build` | Build for production     |
| `npm run lint`  | Run ESLint checks        |

---

## 🤝 Contributing

Feel free to submit issues and enhancement requests!

---

## 📄 License

MIT License - feel free to use this project for your purposes.
