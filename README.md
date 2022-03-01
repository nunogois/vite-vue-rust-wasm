# vite-vue-rust-wasm

Example showcasing a new Vite project using Vue 3 + TypeScript + Tailwind CSS + Rust + WebAssembly.

Check out a SvelteKit example [here](https://github.com/nunogois/sveltekit-rust-wasm).

## Quick Start

### Prerequisites

1. First of all, [rustup](https://rustup.rs/) if you haven't already;
2. Update with `rustup update`;
3. Install [wasm-pack](https://rustwasm.github.io/wasm-pack/installer/) if you haven't already;
4. Globally install [cargo-watch](https://crates.io/crates/cargo-watch) with `cargo install cargo-watch` or `cargo binstall cargo-watch`;

### Project

1. Setup the project (install dependencies and build wasm): `yarn setup`;
2. Run the project: `yarn dev`;
3. Build the project for release: `yarn build`;

## Dev Log

1. Created Vite + Vue3 + TS project with `npm init vite vite-vue-rust-wasm`;
2. Added Tailwind CSS as per [these instructions](https://tailwindcss.com/docs/guides/vite);
3. Created `wasm` package with `wasm-pack new wasm`;
4. Installed [vite-plugin-wasm-pack](https://github.com/nshen/vite-plugin-wasm-pack) with `yarn add -D vite-plugin-wasm-pack` and added `wasm` package in `vite.config.ts`;
5. Added relevant scripts to `package.json`;
6. Added Vue component `HelloWasm.vue` with WebAssembly example;

# Vue 3 + Typescript + Vite

This template should help get you started developing with Vue 3 and Typescript in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

## Recommended IDE Setup

- [VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=johnsoncodehk.volar)

## Type Support For `.vue` Imports in TS

Since TypeScript cannot handle type information for `.vue` imports, they are shimmed to be a generic Vue component type by default. In most cases this is fine if you don't really care about component prop types outside of templates. However, if you wish to get actual prop types in `.vue` imports (for example to get props validation when using manual `h(...)` calls), you can enable Volar's `.vue` type support plugin by running `Volar: Switch TS Plugin on/off` from VSCode command palette.
