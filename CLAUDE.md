# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an Astro-based minimal blog theme called "Chiri" built for personal blogging with features like dark mode, MDX support, KaTeX math rendering, and customizable UI components.

## Commands

### Development
- `pnpm dev` - Start development server
- `pnpm build` - Build for production (includes prebuild script)
- `pnpm preview` - Preview production build
- `pnpm lint` - Run ESLint
- `pnpm lint:fix` - Fix ESLint errors
- `pnpm format` - Format code with Prettier
- `pnpm format:check` - Check code formatting

### Content Management
- `pnpm new <title>` - Create new post (use `_title` for drafts)
- `pnpm update-theme` - Update theme to latest version

## Architecture

### Content Collections
- **Posts**: Located in `src/content/posts/` - supports both `.md` and `.mdx` files
- **About**: Located in `src/content/about/` - markdown files for about page content
- Content schema defined in `src/content.config.ts` with frontmatter validation

### Component Structure
- **Layouts**: `src/layouts/` - BaseLayout, PostLayout, IndexLayout
- **UI Components**: `src/components/ui/` - reusable components like ThemeToggle, TableOfContents, LinkCard
- **Layout Components**: `src/components/layout/` - Header, Footer, BaseHead
- **Widgets**: `src/components/widgets/` - PostList, About, FormattedDate
- **Examples**: `src/components/examples/` - demo components for theme showcase

### Configuration
- **Main config**: `src/config.ts` - theme settings, site info, post options
- **Astro config**: `astro.config.ts` - build configuration with custom plugins
- Uses Netlify adapter by default (configurable for other platforms)

### Custom Plugins
- `src/plugins/` contains custom Astro plugins:
  - `remark-embedded-media.mjs` - embedded content support
  - `remark-reading-time.mjs` - reading time calculation
  - `remark-toc.mjs` - table of contents generation
  - `rehype-image-processor.mjs` - image processing
  - `rehype-copy-code.mjs` - copy code functionality

### Key Features
- Content-driven with Astro Content Collections
- MDX support with custom components
- KaTeX math rendering
- Custom markdown plugins for enhanced functionality
- Responsive design with light/dark themes
- RSS/Atom feeds and sitemap generation
- OpenGraph meta tags for social sharing

### File Structure Notes
- Static assets in `public/`
- Content assets in `src/content/posts/_assets/`
- Global styles in `src/styles/`
- TypeScript types in `src/types/`
- Utility functions in `src/utils/`