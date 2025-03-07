# ComfyUI Wiki 工作流仓库
🌐 多语言支持: [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

本仓库存储[ComfyUI-Wiki.com](https://comfyui-wiki.com/zh)的所有工作流文件。每个工作流包含预览图（含元数据）和JSON文件，均可直接拖入ComfyUI加载。

## 开始使用

### 环境要求
- 已安装 [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
- 新用户请参考[ComfyUI Wiki安装指南](https://comfyui-wiki.com/zh/install/install-comfyui)

## 缺失模型处理
加载工作流时将自动检测缺失模型：
![缺失模型提示](/readme_images/missing_models.png)

### ComfyUI桌面版用户
1. 点击弹窗中的下载按钮
2. 注意事项：
   - 仅支持CivitAI和Hugging Face模型
   - 确保网络可访问上述平台
   - .pth等不安全格式需手动下载

### 其他版本用户
1. 浏览器下载后需手动移动文件至`ComfyUI/models/`

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

### 安装指南
![ComfyUI Manager界面](/readme_images/comfyui_manger.png)
1. 点击`Manager`按钮
2. 选择`Install missing nodes`
3. 点击弹窗中的`Install`

![节点安装示例](/readme_images/install_missing_nodes.jpg)

### 重要提示
- 自动安装需访问GitHub
- 受限网络用户请参考[手动安装指南](https://comfyui-wiki.com/zh/install/install-custom-nodes)
- 各工作流README提供专属节点信息

> 所有工作流均通过安全检查，请从官方渠道获取模型 