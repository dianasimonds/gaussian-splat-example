# Scene Viewer

A standalone viewer for your exported Marble scene, powered by [SparkJS](https://sparkjs.dev).

## Quickstart

To view your scene locally, you'll need to serve the files over HTTP (opening `index.html` directly won't work).

### Using VS Code Live Server

If you're using VS Code, a simple option is the Live Server extension.

1. Install the `Live Server` extension in VS Code.
2. Open this folder in VS Code.
3. Right-click `index.html` and choose `Open with Live Server`.

### Using Python

The easiest way is to use Python's built-in HTTP server:

```bash
# Navigate to this folder in your terminal
cd /path/to/your/exported/scene

# Start the server
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in your browser.

### Using Node.js

Alternatively, if you have Node.js installed:

```bash
npx serve .
```

## Files

- `index.html` – Main scene viewer
- `audio.html` – Scene viewer with audio support
- `splat-audio.html` – Splat viewer with positional audio markers
- `marble-template.html` – Base template file
- `scene.json` – Scene data and transforms
- `spark.module.min.js` – SparkJS library
- `audio/` – Audio files used by the examples
- `splats/` – Gaussian splat assets

## Resources

For more information on SparkJS and its capabilities, here are some places to start:

- **SparkJS Documentation**: https://sparkjs.dev/docs
- **SparkJS Examples (Demos)**: https://sparkjs.dev/examples/ 
- **SparkJS Examples (Source Code)**: https://github.com/sparkjsdev/spark/tree/main/examples
- **SparkJS Discord**: https://discord.gg/DxubkP8D