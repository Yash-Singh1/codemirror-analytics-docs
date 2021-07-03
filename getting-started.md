# Getting Started

This guide will help you getting started with CodeMirror Analytics.

## Installation

```sh
npm install codemirror-plugin-analytics
```

## Token Setup

1. Goto <https://codemirror-analytics-backend.epiccodewizard.repl.co/>
2. Sign in with your Replit account
3. Copy the secret on your dashboard

## Client-side Setup

1. Import the `index.js` of the package in a script tag
2. Run the following after importing `index.js` (assuming `editor` is the instance)

```js
editor.on('optionChange', CodemirrorAnalyticsHooks('THE_SECRET_YOU_COPIED').optionChange);
```
