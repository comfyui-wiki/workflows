# ComfyUI Wiki Workflows
🌐 Multilingual Support: [中文](README.zh.md) | [Español](README.es.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

This repository stores all workflow files for [ComfyUI-Wiki.com](https://comfyui-wiki.com/en). Each workflow includes a preview image (with embedded metadata) and a JSON file. Both formats can be dragged directly into ComfyUI for loading.

## Getting Started

### Prerequisites
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) installed
- For new installations, follow the [ComfyUI Wiki Installation Guide](https://comfyui-wiki.com/en/install/install-comfyui)

## Handling Missing Models
When loading workflows, ComfyUI will automatically detect and prompt for missing models:
![Missing models prompt](/readme_images/missing_models.png)

### For ComfyUI Desktop Users
1. Click the download button in the prompt dialog
2. Important notes:
   - Only supports models from [CivitAI](https://civitai.com) and [Hugging Face](https://huggingface.co/)
   - Ensure network access to these platforms
   - Unsupported file types (e.g., .pth) will have separate instructions

### For Other Versions (Portable/Manual Installations)
1. Downloaded files will be saved by your browser
2. Manually move files to corresponding subdirectories in `ComfyUI/models/`

Example structure after setup:
```bash
ComfyUI/
└── models/
    ├── checkpoints/
    │   └── dreamshaper_8.safetensors
    └── loras/
        ├── blindbox_ViMix.safetensors
        └── MoXinV1.safetensors
```
> Restart/refresh ComfyUI after moving files

## Resolving Missing Nodes
![Missing nodes prompt](/readme_images/missing_node_types.png)

### Troubleshooting Steps
1. **Core nodes missing**: [Update ComfyUI](https://comfyui-wiki.com/en/tutorial/basic/how-to-update-comfyui)
2. **Custom nodes missing**: Install via ComfyUI Manager

### Installation Guide
![ComfyUI Manager interface](/readme_images/comfyui_manger.png)
1. Click the `Manager` button in ComfyUI
2. Select `Install missing nodes`
3. Click `Install` in the dialog

![Node installation demo](/readme_images/install_missing_nodes.jpg)

### Important Notes
- Requires GitHub access for automatic installations
- Manual installation guide available for restricted networks: [Custom Nodes Installation](https://comfyui-wiki.com/en/install/install-custom-nodes)
- Workflow-specific node information provided in individual README files

> All workflows undergo security checks. Obtain models only from official sources.