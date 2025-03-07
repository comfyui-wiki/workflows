# ComfyUI Wiki Workflows
🌐 Multilingual Support: [中文](README.zh.md) | [Español](README.es.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [한국어](README.ko.md)
This repository contains all workflow files for [ComfyUI-Wiki.com](https://comfyui-wiki.com/zh). Each workflow includes a preview image (with metadata) and JSON file, which can be directly dragged into ComfyUI for loading.

## Getting Started

After downloading corresponding models, drag them into ComfyUI to load the workflow. Each workflow file contains a readme.md with model download information.

### Requirements
- Have [ComfyUI](https://github.com/comfyanonymous/ComfyUI) installed
- New users please refer to [ComfyUI Wiki Installation Guide](https://comfyui-wiki.com/zh/install/install-comfyui)

## Handling Missing Models
ComfyUI will automatically detect missing models when loading workflows:
![Missing models prompt](/readme_images/missing_models.png)

### For ComfyUI Desktop Users
1. Click the download button in the pop-up window
2. Notes:
   - Currently only supports model detection from CivitAI and Hugging Face
   - Ensure network access to these platforms
   - Unsupported formats like .pth will be recorded in readme.md for manual download

### For Other Versions

1. Click the `Download` button to initiate browser download, then manually move files to `ComfyUI/models/`

Example directory structure:
```bash
ComfyUI/
└── models/
    ├── checkpoints/
    │   └── dreamshaper_8.safetensors
    └── loras/
        ├── blindbox_ViMix.safetensors
        └── MoXinV1.safetensors
```
> After moving files, please restart/refresh the interface

## Handling Missing Nodes
![Missing nodes prompt](/readme_images/missing_node_types.png)

### Solutions
1. **Core nodes missing**: [Update ComfyUI](https://comfyui-wiki.com/zh/tutorial/basic/how-to-update-comfyui)
2. **Custom nodes missing**: Install via ComfyUI Manager

### ComfyUI Manager Installation Guide
![ComfyUI Manager interface](/readme_images/comfyui_manager.png)
1. Click the `Manager` button
2. Select `Install missing nodes`
3. Click `Install` in the pop-up window

![Node installation example](/readme_images/install_missing_nodes.jpg)

### Important Notes
- Automatic node installation requires GitHub access
- Restricted network users please refer to [Manual Installation Guide](https://comfyui-wiki.com/zh/install/install-custom-nodes)
- Each workflow's README provides URLs for custom nodes


by [@ComfyUI-Wiki](https://github.com/comfyui-wiki) | [ComfyUI-Wiki](https://comfyui-wiki.com/zh)
