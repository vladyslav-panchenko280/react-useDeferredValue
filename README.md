# Deferred Value Demo

A React demo showcasing `useDeferredValue` for handling expensive renders without blocking the UI.

## Features

- Image filter controls (blur, brightness, contrast, saturate, sepia)
- Simulated expensive render (100ms delay) to demonstrate concurrent features
- Uses `useDeferredValue` to defer updates to expensive components

## Getting Started

```bash
npm install
npm run dev
```

## How It Works

The `DisplayImage` component simulates an expensive render. Without concurrent features, moving sliders would freeze the UI. With `useDeferredValue`, React prioritizes slider responsiveness and defers the image re-renders.
