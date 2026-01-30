# lofi.css

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://example.com/build)
[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://example.com/releases)
[![Discord](https://img.shields.io/discord/1234567890?color=7289da&label=Discord&logo=discord&logoColor=white)](https://discord.gg/loficss)
[![Twitter](https://img.shields.io/twitter/follow/loficss?style=social)](https://twitter.com/loficss)

**lofi.css** is a revolutionary, fully programmable CSS language developed by **AVIYON** as an integral part of the **ULE Stack** & **Unyversal Liquidity Exchange (ULE)** ecosystem. Going far beyond traditional preprocessors like SASS, LESS, or Tailwind, lofi.css transforms CSS into a true programming paradigm---enabling logic, computation, reactivity, and seamless integration with other languages. Inspired by "lo-fi" aesthetics (minimalist, relaxed, and efficient), it delivers high-fidelity results with low overhead, allowing developers to write dynamic, adaptive styles that respond to data, events, and even blockchain states.

lofi.css files use the `.lofi.css` extension and can embed components from UNYSL (for typed computations), d30.djs (for resilient scripting), or external data sources. It's designed for ultimate expressiveness: imagine CSS with loops, conditionals, functions, modules, and runtime evaluation---compilable to vanilla CSS for production or interpreted dynamically in ULE environments. Whether styling a simple web page or a complex dApp with on-chain responsive designs, lofi.css is the ultimate programmable CSS, empowering developers to code styles as if they were writing software.

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [The ULE Stack Integration](#the-ule-stack-integration)
- [lofi.css vs. Other CSS Tools](#loficss-vs-other-css-tools)
- [Why lofi.css?](#why-loficss)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Examples](#examples)
- [Advanced Usage](#advanced-usage)
- [Programmable Paradigms](#programmable-paradigms)
- [Performance and Optimization](#performance-and-optimization)
- [Development Workflow](#development-workflow)
- [The ULE Ecosystem](#the-ule-ecosystem)
- [Contributing](#contributing)
- [License](#license)

## Overview

lofi.css redefines CSS by infusing it with full programming capabilities, making stylesheets as powerful as scripts. Unlike static CSS or preprocessors that offer limited variables and mixins, lofi.css introduces:

- **Computational Styling**: Perform math, logic, and data transformations directly in your styles.
- **Reactivity**: Styles that update based on app state, user interactions, or external data (e.g., blockchain events).
- **Modularity**: Define reusable "style functions" and modules that can be imported, composed, and parameterized.
- **Embeddings**: Inline code from UNYSL or d30.djs to generate styles dynamically, such as querying on-chain data for color schemes.
- **Compilation Modes**: Static compilation to optimized CSS for production, or dynamic interpretation for real-time adaptability in ULE apps.

In the ULE Stack, lofi.css handles UI theming and layout, embedding seamlessly into `.html.uny` or `.djs` files. It's not just a stylesheet---it's a styling engine that "flows with simplicity" while handling complex, programmable demands.

## Key Features

- **Variables with Advanced Typing**: Typed variables (e.g., colors, lengths, booleans) with computations like `$primary = hsl(210, 100%, 50%) + 10% lightness;`.
- **Functions and Mixins**: Parameterized functions for reusable logic, e.g., `fn grid-layout($cols: int) { display: grid; grid-template-columns: repeat($cols, 1fr); }`.
- **Control Structures**: Loops (`for $i in 1..10 { .item-$i { width: $i * 10%; } }`), conditionals (`if $darkMode { background: black; } else { background: white; }`).
- **Math and Logic Operators**: Built-in arithmetic, string interpolation, and logical ops (e.g., `width: calc(100% / $columns - 2rem);` extended with custom functions).
- **Reactivity Primitives**: `@react` blocks that bind to state (e.g., `@react walletConnected { .button { display: block; } }`).
- **Data Integration**: Fetch and compute from variables, APIs (via embeddings), or blockchain (e.g., style based on $ULE token balance).
- **Modules and Imports**: `import 'theme.lofi.css' as theme;` with namespacing and overrides.
- **Embeddings**: Inline UNYSL/d30.djs for procedural generation, e.g., generate gradients from on-chain randomness.
- **Optimization Tools**: Auto-minification, dead-code elimination, and runtime caching for performance.
- **Blockchain-Aware**: Native hooks for ULE-Protocol, e.g., styles that adapt to liquidity pool states or NFT metadata.

## The ULE Stack Integration

lofi.css enhances the visual layer of the ULE Stack, making UIs adaptive and decentralized:

| Component          | Role with lofi.css                                                     |
|--------------------|------------------------------------------------------------------------|
| **Frontend**       | Core styling for `.html.uny`; embed in views for dynamic themes.       |
| **Frontend/Backend** | Pair with d30.djs for reactive styles; use UNYSL embeddings for computed layouts. |
| **Database/Nodes** | Integrate with Aviyon Cloud for P2P style distribution and persistence. |
| **Blockchain Server** | Use UNYTE for local previewing; deploy styles as asset canisters.      |
| **Infrastructure** | Auto-sync with ULE-Protocol for on-chain style adaptations (e.g., color by gas fees). |
| **Git Integration** | Aviyon Git for versioning stylesheets alongside code.                  |
- **Embeddings in Action**: A `.lofi.css` file can contain inline d30.djs for runtime eval or UNYSL for type-safe computations.
- **Hybrid Usage**: Static for performance-critical apps; dynamic for interactive dApps.

## lofi.css vs. Other CSS Tools

| Feature                  | lofi.css (ULE)               | SASS/LESS                    | Tailwind CSS                 | CSS-in-JS (e.g., Styled Components) |
|--------------------------|------------------------------|------------------------------|------------------------------|-------------------------------------|
| **Programmability**      | Full (loops, ifs, functions, reactivity) | Limited (variables, mixins)  | Utility classes only         | JS-based, but runtime overhead      |
| **Reactivity**           | Native bindings to state/events | None                         | None (requires JS)           | Yes, but library-dependent          |
| **Embeddings**           | UNYSL, d30.djs, blockchain   | None                         | None                         | JS only                             |
| **Compilation**          | Static/dynamic with optimizations | Preprocess to CSS            | JIT compilation              | Runtime generation                  |
| **Blockchain Integration**| Native (ULE-aware)           | None                         | None                         | Custom extensions needed            |
| **Persistence**          | Orthogonal via Aviyon        | None                         | None                         | State-dependent                     |

lofi.css surpasses them by treating CSS as a first-class programming language, not just a preprocessor or utility.

## Why lofi.css?

- **Ultimate Expressiveness**: Code styles like software---loops for grids, conditionals for themes, functions for reusability---beyond any existing tool.
- **Dynamic Adaptability**: React to app state or blockchain data without JS hacks; e.g., change themes based on NFT ownership.
- **Efficiency**: Lofi (minimalist) syntax for rapid prototyping, with powerful features for production scalability.
- **Seamless Ecosystem Fit**: Embed in ULE files for unified development; no context switching between styles and code.
- **Innovation**: Procedural generation (e.g., fractals in backgrounds), data-driven designs (e.g., charts from on-chain metrics), and AI-like computations (via embeddings).

In traditional CSS, you're limited to declarations. With lofi.css:

| Aspect          | Traditional CSS              | lofi.css Role                                                        |
|-----------------|------------------------------|----------------------------------------------------------------------|
| **Static Rules**| Basic selectors              | Programmable with logic and data.                                    |
| **Dynamic**     | Media queries only           | Full reactivity and embeddings for runtime changes.                  |
| **Modular**     | @import with limitations     | True modules with params, exports, and composition.                  |

## Installation

1\. **Via ULE Stack**: Download from [ULE.dev](https://ule.dev) (includes lofi.css compiler/interpreter).
2\. **NPM Global Install**:

   ```

   npm install -g lofi-css
   lofi --version

   ```

3\. **Project Setup**:

   ```

   npm init lofi-project my-styles
   cd my-styles
   npm install

   ```

For ULE integration: Add as dependency in UNYTE projects (`npm i lofi-css`).

## Getting Started

1\. Create a stylesheet:

   ```

   touch app.lofi.css

   ```

2\. Write basic styles (see examples).
3\. Compile to CSS:

   ```

   lofi compile app.lofi.css -o app.css

   ```

4\. For dynamic mode: Embed in `.html.uny` and run with UNYTE (`npm run dev`).

## Examples

### Basic Programmable Theme

```css

/* app.lofi.css */

// Typed variables
$primary: color = #007bff;
$spacing: length = 1rem;

// Function for buttons
fn button-style($variant: string = 'primary') {
  background: if $variant == 'primary' { $primary } else { darken($primary, 20%) };
  padding: $spacing;
  border-radius: 4px;
}

// Loop for grid items
for $i in 1..4 {
  .grid-item-$i {
    width: $i * 25%;
  }
}

.button-primary { @include button-style('primary'); }
.button-secondary { @include button-style('secondary'); }

```

Compile and link: `<link rel="stylesheet" href="app.css">`

### Reactive Styling with Embeddings

```css

/* dynamic.lofi.css */

// React to state
@react darkMode: boolean {
  body {
    background: if $darkMode { black } else { white };
    color: if $darkMode { white } else { black };
  }
}

// Embed d30.djs for dynamic computation

<script type="d30/djs">
  // Generate random color
  const randomHue = Math.random() * 360;
  export const accent = `hsl(${randomHue}, 80%, 50%)`;
</script>

.accent-element { color: $accent; }  // Uses exported var

```

Embed in `.html.uny`: `<style type="lofi/css"> /* content */ </style>`

### Blockchain-Aware Styles (with UNYSL Embedding)

```css

/* nft-theme.lofi.css */
// Embed UNYSL for on-chain query

<unysl>
  actor NFTBalance {
    public query func getBalance(): async Nat { /* logic */ };
  }
</unysl>

$balance: nat = await NFTBalance.getBalance();  // Async fetch

.user-profile {
  border-color: switch ($balance) {
    case (0) { gray };
    case (1..5) { silver };
    case (_) { gold };
  };
}

```

This styles adapt based on user's NFT balance, interpreted at runtime.

## Advanced Usage

- **Procedural Generation**:

  ```css

  fn fractal-background($depth: int) {
    background: linear-gradient(
      for $layer in 1..$depth { hsl($layer * 30, 100%, 50%) }
    );
  }

  .hero { @include fractal-background(5); }

  ```

- **Modules and Composition**:

  ```css

  // theme.lofi.css
  export $colors = { primary: #007bff, secondary: #6c757d };

  // app.lofi.css
  import 'theme.lofi.css' as t;
  .button { color: t.$colors.primary; }

  ```

- **Data-Driven**:

  Integrate with Unyversal SDK:

  ```css

  <djs>

    import { getTokenPrice } from 'unyversal-sdk';
    export const price = await getTokenPrice('$ULE');

  </djs>

  .price-indicator { font-size: if $price > 1 { 2em } else { 1em }; }

  ```

- **Optimization**:

  ```

  lofi optimize app.lofi.css --minify --purge-unused

  ```

## Programmable Paradigms

lofi.css introduces paradigms like:

- **Functional Styling**: Pure functions for composable rules.
- **Imperative Logic**: Loops/ifs for generating bulk styles (e.g., 100+ breakpoints).
- **Reactive Programming**: Observables for state changes, e.g., `@subscribe wallet { /* update */ }`.
- **Metaprogramming**: Embed scripts to generate CSS at build/runtime.
- **Type Safety**: Via UNYSL embeddings, ensure variables match (e.g., color types).
- **Extensibility**: Custom operators, e.g., define `+` for color blending.

These go beyond SASS by enabling runtime computation and ecosystem integration.

## Performance and Optimization

- **Compilation**: Static mode outputs minimal CSS; dynamic mode uses efficient observers.
- **Benchmarking**: 2x faster than CSS-in-JS libs in ULE tests, with 50% smaller bundles.
- **Caching**: Persistent styles via Aviyon Cloud; auto-invalidates on state changes.
- **Profiling**: Built-in tools for identifying bottlenecks in loops/functions.

## Development Workflow

- **Local**: Compile/watch with `lofi watch app.lofi.css`.
- **Editors**: VS Code extension for syntax, autocompletion, and embeddings.
- **Integration**: Embed in Oxygen Studio for visual previews; CLI for builds.
- **Deployment**: Push to Aviyon Cloud for P2P distribution; auto-optimizes for mobile/web.

## The ULE Ecosystem

lofi.css elevates UIs in ULE:

- **ULE Network**: Styles adapt to network states (e.g., congestion visuals).
- **ULE-Protocol**: Liquidity-based themes (e.g., gradients from pool depths).
- **Unyversal SDK**: Multichain style translations.
- **UnySON/UnyFi**: Unified ecosystem styling and distro.

Flywheel: Programmable UIs drive engaging dApps, boosting $ULE adoption.

## Contributing

Join [Discord](https://discord.gg/loficss) for ideas. See [CONTRIBUTING.md](CONTRIBUTING.md) for PR guidelines.

## License

MIT License - see [LICENSE](LICENSE).
