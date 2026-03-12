# React Native Optimization Guide

This repo contains **"The Ultimate Guide to React Native Optimization (2026)"** by Callstack as a PDF. It is a learning resource for React Native developers covering performance optimization across JavaScript, native, and bundling layers.

## How Claude should help

At the start of a conversation, read the entire book by converting it to text (`pdftotext` via Bash) and reading the full output. This ensures you can answer questions accurately without needing to re-extract sections later.

Assist users in learning its content: explaining concepts, answering questions, quizzing, summarizing chapters, and connecting ideas across sections.

## Reading the PDF

The PDF can be extracted via Bash:

```bash
pdftotext "The Ultimate Guide to React Native Optimization (2026).pdf" -
```

This requires `poppler` to be installed:
- **macOS**: `brew install poppler`
- **Linux**: `apt-get install poppler-utils`

Note: The Read tool may not find `pdftoppm` due to PATH issues. Use `pdftotext` via Bash as the reliable method.

## Book structure

The book is organized around two key metrics: **TTI** (Time to Interactive) and **FPS** (Frames Per Second).

### Part 1: JavaScript
- How to Profile JS and React Code
- How to Measure JS FPS
- How to Hunt JS Memory Leaks
- Uncontrolled Components
- Higher-Order Specialized Components
- Atomic State Management
- Concurrent React
- React Compiler
- High-Performance Animations Without Dropping Frames

### Part 2: Native
- Understand Platform Differences
- How to Profile Native Parts of React Native
- How to Hunt Memory Leaks
- How to Measure TTI
- Understanding Native Memory Management
- Understand the Threading Model of Turbo Modules and Fabric
- Use View Flattening
- Use Dedicated React Native SDKs Over Web
- Make Your Native Modules Faster

### Part 3: Bundling
- How to Analyze JS Bundle Size
- How to Analyze App Bundle Size
- Determine True Size of Third-Party Libraries
- Avoid Barrel Exports
- Experiment With Tree Shaking
- Load Code Remotely When Needed
- Shrink Code With R8 Android
- Use Native Assets Folder
- Disable JS Bundle Compression

## Example prompts

- "Explain the chapter on memory leaks"
- "Quiz me on Part 1"
- "Summarize the bundling section"
- "What's the difference between JS and native memory leaks?"
- "How do I measure TTI in React Native?"
- "What are the best practices for animations?"
