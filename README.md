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

## ComfyUI Manager and Registry

This repo is now prepared for Comfy Registry publishing, which is what powers ComfyUI Manager discovery.

Automatic publishing is configured via [`.github/workflows/publish_action.yml`](.github/workflows/publish_action.yml). To make it live in the registry and appear in Manager:

1. Create a publisher at [registry.comfy.org](https://registry.comfy.org)
2. Confirm the publisher id is `ihorpankin`, or update `PublisherId` in [`pyproject.toml`](pyproject.toml) before first publish
3. Create a registry publishing API key
4. Add it to this GitHub repo as the `REGISTRY_ACCESS_TOKEN` secret
5. Bump the version in [`pyproject.toml`](pyproject.toml) and push to `master`

You can also publish manually with:

```bash
comfy node publish
```

## Repository

- GitHub: https://github.com/ihorpankin/comfyui-link
- Issues: https://github.com/ihorpankin/comfyui-link/issues
