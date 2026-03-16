# theme-switch-animation

Simple browser demo showing animated light/dark theme switching with the View Transitions API.

## What it is

This project is a single HTML demo that toggles between light and dark mode and animates the transition in the browser.

File:

```text
index.html
```

## Features

- light/dark theme toggle
- uses `document.startViewTransition`
- fallback theme toggle when the API is not supported
- multiple transition styles:
  - circle reveal
  - diagonal reveal
  - left-to-right reveal
  - shutter reveal
- built with plain HTML, CSS, JavaScript, and Tailwind CDN

## How it works

According to MDN, `document.startViewTransition()` starts a same-document view transition by capturing the current view, running an update callback, and then animating from the old view to the new one. The `::view-transition-new(root)` pseudo-element represents the new state of the page during that transition, so applying an animation there controls how the updated theme is revealed on screen.

<a href="https://developer.mozilla.org/en-US/docs/Web/API/Document/startViewTransition" target="_blank" rel="noopener noreferrer">Know more</a>

## Run

Open [index.html](https://addevin.github.io/theme-switch-animation/index.html) in a browser.

## Notes

- Best experience requires a browser that supports `document.startViewTransition`
- Tailwind is loaded from CDN
- The demo includes a link to the MDN View Transitions API documentation

## Links

<a href="https://developer.mozilla.org/en-US/docs/Web/API/Document/startViewTransition" target="_blank" rel="noopener noreferrer">MDN: Document.startViewTransition()</a>
