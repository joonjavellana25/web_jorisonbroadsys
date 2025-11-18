# JBS One Svelte Web App

This is a web app for JBS One, built using [SvelteKit](https://kit.svelte.dev/).

## Installation

You will need to install Node.js and npm, or Bun. You can download them from:
- Node.js: https://nodejs.org/en/download/
- Bun: https://bun.sh/

### Installing a SvelteKit Project

You can create a new SvelteKit project using any of the following methods:

#### Using Bun (Recommended)
```bash
bunx sv create jbs-one-app
cd jbs-one-app
bun --bun run dev
```

#### Using Node.js/npm
```bash
npm create svelte@latest jbs-one-app
cd jbs-one-app
npm install
```

#### Alternative methods
```bash
# Using yarn
yarn create svelte jbs-one-app
cd jbs-one-app
yarn install

# Using pnpm
pnpm create svelte jbs-one-app
cd jbs-one-app
pnpm install
```

During the setup process, you'll be prompted to choose:
- Project template (skeleton, demo, etc.)
- TypeScript support
- Additional features (ESLint, Prettier, Playwright, etc.)

### Prerequisites
- Node.js (version 18 or higher recommended) OR Bun (latest version)
- npm, yarn, pnpm, or bun package manager

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd jbs-one-svelte-app
   ```

2. **Install dependencies**
   ```bash
   # Using bun (recommended)
   bun install
   
   # Or using npm
   npm install
   ```

3. **Start the development server**
   ```bash
   # Using bun
   bun run dev
   
   # Using npm
   npm run dev
   ```
   
   Alternatively, start the server and open the app in a new browser tab:
   ```bash
   bun run dev -- --open
   ```

## Available Scripts

### Using Bun
```bash
bun run dev        # Start the development server
bun run build      # Build the app for production
bun run preview    # Preview the production build locally
bun run check      # Run Svelte checks and validate code
bun run test       # Run the test suite (if configured)
```

### Using npm
```bash
npm run dev        # Start the development server
npm run build      # Build the app for production
npm run preview    # Preview the production build locally
npm run check      # Run Svelte checks and validate code
npm run test       # Run the test suite (if configured)
```

## Project Structure

```
jbs-one-svelte-app/
├── src/
│   ├── routes/           # File-based routing
│   ├── lib/             # Reusable components and utilities
│   ├── app.html         # Main HTML template
│   └── app.css          # Global styles
├── static/              # Static assets (images, fonts, etc.)
├── package.json
└── svelte.config.js     # SvelteKit configuration
```

## Environment Variables

Create a `.env` file in the root directory for environment-specific variables:

```env
# .env
VITE_API_BASE_URL=your_api_url_here
```

## Building for Production

To create a production build:

```bash
# Using bun
bun run build

# Using npm
npm run build
```

You can preview the production build with:
```bash
bun run preview
# or
npm run preview
```

## Why Use Bun?

Bun offers several advantages for SvelteKit development:
- **Faster installs**: Significantly faster dependency installation
- **Quick startup**: Faster development server startup times
- **Built-in tools**: Includes test runner, package manager, and bundler
- **Better performance**: Generally faster execution for scripts and builds
- **bunx**: Faster alternative to npx for running packages

## Deployment

This SvelteKit app can be deployed to various platforms:

- **Vercel**: `bun run build` and deploy the output
- **Netlify**: Use the `@sveltejs/adapter-netlify` adapter
- **Static hosting**: Use `@sveltejs/adapter-static` for static sites

## Technologies Used

- [SvelteKit](https://kit.svelte.dev/) - Full-stack web framework
- [Svelte](https://svelte.dev/) - Component framework
- [Vite](https://vitejs.dev/) - Build tool and dev server
- [Bun](https://bun.sh/) - Fast JavaScript runtime (optional)

## Contributing

Please read our contributing guidelines before submitting pull requests.

## License

[Add your license information here]

## Support

For support and questions, please contact [your support contact].