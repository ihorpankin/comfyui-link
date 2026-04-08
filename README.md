# Comfy Link

Comfy Link is a ComfyUI custom node and Photoshop UXP bridge that sends the Photoshop canvas and selection mask to ComfyUI, runs a workflow, and returns the result as a new Photoshop smart object layer.

## Install

### Manual install

1. Clone this repo into `ComfyUI/custom_nodes/comfyui-link`
2. Install dependencies in your ComfyUI Python environment:

```bash
pip install -r requirements.txt
```

3. Restart ComfyUI
4. Load or reload the Photoshop plugin from `photoshop/manifest.json` in the UXP Developer Tool

## What it includes

- `Receive from Photoshop` node
- `Send to Photoshop` node
- Bridge server routes under `/ps-bridge`
- Photoshop UXP panel in `photoshop/`

## Repository

- GitHub: https://github.com/ihorpankin/comfyui-link
- Issues: https://github.com/ihorpankin/comfyui-link/issues
