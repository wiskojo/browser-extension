# ChatGPT Wake Word Voice Assistant Browser Extension for Google Chrome

This is the source code for building the ChatGPT Wake Word Voice Assistant Browser Extension for Google Chrome. It uses Picovoice Porcupine for wake word detection + SpeechRecognitionAPI to perform a query to ChatGPT via voice.

This is a very simple POC extended from Picovoice's [`browser-extension`](https://github.com/Picovoice/browser-extension).

You will need your own Picovoice AccessKey which can be acquired at the [`Picovoice console`](https://console.picovoice.ai/).

## Compatibility

- Google Chrome (57)

## Prerequisites

- yarn (or npm)

## Install dependencies

```console
yarn
```

(or)

```console
npm install
```

## Build

```console
yarn build
```

(or)

```console
npm run build
```

### Update live with webpack

```console
yarn run webpack -w
```

## Run locally

After building, the `extension` subdirectory is the artifact provide to Chrome.

1. You will need to enable developer mode in Chrome, since the source version of the extension is not delivered from the Chrome Store.
1. In Chrome, go to `chrome://extensions`. Press "Load Unpacked" and then select the `extension` folder.
1. Press the blue button on the extension to activate it. (Chrome may hide this behind the "Puzzle Piece" icon.)
