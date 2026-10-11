# Hand Tracking Air Canvas

A browser-based drawing prototype controlled by hand gestures through a webcam. This is a group project; the original code and its history are in [sucsage/ConOps](https://github.com/sucsage/ConOps).

## Try it locally

Run a local web server from this directory:

```bash
python3 -m http.server 8000
```

Open <http://localhost:8000>, select **Start Camera**, and allow camera access. The page loads MediaPipe from a CDN, so an internet connection is needed to load the hand-tracking library.

## Controls

| Action | Control |
| --- | --- |
| Toggle drawing mode | Shift |
| Draw | Raise one finger while drawing mode is on |
| Pause the current stroke | Raise two or more fingers |
| Clear the canvas | Space or **Clear Canvas** |
| Change color or brush size | Use the side panel |

The interface shows hand landmarks and live FPS, stroke, point, and hand counts. Drawings stay in memory for the current session and disappear when the page is refreshed.

## Project document

The group [Software Requirements Specification](docs/Hand-Tracking-Air-Canvas-SRS.pdf) describes the requirements, interface, and system limitations.

## Built with

HTML, CSS, JavaScript, HTML Canvas, and MediaPipe Hands.
