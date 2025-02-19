---
title: CanvasCaptureMediaStreamTrack.canvas
slug: Web/API/CanvasCaptureMediaStreamTrack/canvas
page-type: web-api-instance-property
tags:
  - Canvas
  - CanvasCaptureMediaStreamTrack
  - Experimental
  - Frame Capture
  - Media Capture
  - Property
  - Read-only
  - Reference
  - Web
browser-compat: api.CanvasCaptureMediaStreamTrack.canvas
---
{{APIRef}}

The {{domxref("CanvasCaptureMediaStreamTrack")}} **`canvas`**
read-only property returns the {{domxref("HTMLCanvasElement")}} from which frames are
being captured.

## Value

An `HTMLCanvasElement` indicating the canvas which is the source of the
frames being captured.

## Example

```js
// Find the canvas element to capture
var canvasElt = document.getElementsByTagName("canvas")[0];

// Get the stream
var stream = canvasElt.captureStream(25); // 25 FPS

// Do things to the stream
// …

// Obtain the canvas associated with the stream
var canvas = stream.canvas;
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{domxref("HTMLCanvasElement.captureStream()")}} to create a stream to capture a
  given canvas element.
- {{HTMLElement("canvas")}}
