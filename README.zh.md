# ComfyUI Wiki 工作流仓库
🌐 多语言支持: [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

本仓库存储[ComfyUI-Wiki.com](https://comfyui-wiki.com/zh)的所有工作流文件。每个工作流包含预览图（含元数据）和JSON文件，均可直接拖入ComfyUI加载。

## 开始使用

对应模型下载后拖入ComfyUI即可加载对应工作流，对应工作流文件会包含一个 readme.md 记录对应模型下载信息

### 环境要求
- 已安装 [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
- 新用户请参考[ComfyUI Wiki安装指南](https://comfyui-wiki.com/zh/install/install-comfyui)

## 缺失模型处理
加载工作流时 ComfyUI 将自动检测缺失模型：
![缺失模型提示](/readme_images/missing_models.png)

### ComfyUI桌面版用户
1. 点击弹窗中的下载按钮
2. 注意事项：
   - 目前仅支持来自 CivitAI和Hugging Face 的模型检测
   - 请确保网络可访问上述平台
   - .pth等不支持的格式文件将在 readme.md 中记录需手动下载安装

### 其他版本用户

1. 点击`Download`按钮，浏览器会执行下载，下载完成后需手动移动文件至`ComfyUI/models/`

示例目录结构：
```bash
ComfyUI/
└── models/
    ├── checkpoints/
    │   └── dreamshaper_8.safetensors
    └── loras/
        ├── blindbox_ViMix.safetensors
        └── MoXinV1.safetensors
```
> 移动文件后请重启/刷新界面

## 缺失节点处理
![缺失节点提示](/readme_images/missing_node_types.png)

### 解决方案
1. **核心节点缺失**：[更新ComfyUI](https://comfyui-wiki.com/zh/tutorial/basic/how-to-update-comfyui)
2. **自定义节点缺失**：通过ComfyUI Manager安装

###  ComfyUI Manager 安装自定义节点指南
![ComfyUI Manager界面](/readme_images/comfyui_manager.png)
1. 点击`Manager`按钮
2. 选择`Install missing nodes`
3. 点击弹窗中的`Install`

![节点安装示例](/readme_images/install_missing_nodes.jpg)

### 重要提示
- 自动安装工作流节点需要网络可以正常访问 GitHub
- 受限网络用户请参考[手动安装指南](https://comfyui-wiki.com/zh/install/install-custom-nodes)
- 各工作流的 README 文件提供自定义节点的 URL


by [@ComfyUI-Wiki](https://github.com/comfyui-wiki) | [ComfyUI-Wiki](https://comfyui-wiki.com/zh)