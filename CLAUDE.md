# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static documentation website for building enterprise-scale LLM chatbot applications. It consists of a single self-contained HTML file with inline CSS and JavaScript - no build tools or dependencies required.

## File Structure

- `index.html` - Main documentation file (served by GitHub Pages)
- `llm-chatbot-documentation.html` - Copy of index.html (keep in sync)
- `.nojekyll` - Disables Jekyll processing on GitHub Pages

## Development

**Local preview:** Open `index.html` in any browser - no server needed.

**Make changes:** Edit the HTML file directly. All CSS is in a `<style>` block (~700 lines), all JS is in `<script>` blocks at the end.

**Keep files in sync:** After editing `index.html`, copy it to `llm-chatbot-documentation.html`.

## Deployment

The site is deployed via GitHub Pages at: https://digital-ai-finance.github.io/LLM-based-app/

Push to `main` branch triggers automatic deployment (1-2 minute build time).

## Key CSS Architecture

The styling uses CSS custom properties for theming:
- Light/dark mode via `[data-theme="light|dark"]` on `<html>`
- Spacing: `--space-xs` through `--space-3xl`
- Typography: `--text-xs` through `--text-4xl`
- Layout: `--sidebar-width`, `--content-max-width`

## Content Sections

The documentation has 12 major sections plus appendices:
1. Introduction
2. Architecture
3. Backend (FastAPI)
4. Frontend (React/Next.js)
5. LLM Integration
6. RAG
7. Conversation Management
8. AI Agents
9. Infrastructure
10. Security
11. Cost Optimization
12. Observability
+ Appendices (API reference, config, troubleshooting, glossary)

Each section uses anchor IDs for navigation (e.g., `#architecture-overview`, `#rag-fundamentals`).
