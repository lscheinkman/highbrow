# Highbrow

> HTM 3D Translation Library

Currently under development, does not actually work yet. See design at [DESIGN](DESIGN.md) for motivation and notes. For more up-to-date architecture, build docs below.

## Install

    npm install .

## Test

    npm test

## Build docs

    ./node_modules/.bin/esdoc
    open docs/index.html

## Build Bundle

    npm run build

Installs into `bin/highbrow.bundle.js`.

## Examples

### WEBGL

There is a simple WEBGL example in [`examples/webgl`](examples/webgl/). The [`webgl-rendering-adapter.js`](examples/webgl/webgl-rendering-adapter.js) interfaces with [cell-viz](https://github.com/numenta/cell-viz), an existing platform I've used for HTM cell rendering in THREE.JS. It currently only models one layer and does not yet apply scale or offset, but if you open [`examples/webgl/index.html`](examples/webgl/index.html) in a browser and hold `s` to strafe backward you can see the animated cells.

#### Controls

Use `wasd` to strafe and `←↑→↓` to rotate the camera. Hold `shift` to increase movement and rotation speed.
