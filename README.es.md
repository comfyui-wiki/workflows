# Flujos de trabajo de ComfyUI Wiki
🌐 Soporte multilingüe: [English](README.md) | [中文](README.zh.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

Este repositorio contiene todos los archivos de flujos de trabajo de [ComfyUI-Wiki.com](https://comfyui-wiki.com/es). Cada flujo incluye una vista previa (con metadatos) y un archivo JSON que se puede arrastrar directamente a ComfyUI.

## Primeros pasos

Descargue los modelos correspondientes y arrástrelos a ComfyUI para cargar el flujo de trabajo. Cada archivo de flujo contiene un readme.md con información de descarga del modelo.

### Requisitos del sistema
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) instalado
- Nuevos usuarios consulten la [guía de instalación de ComfyUI Wiki](https://comfyui-wiki.com/es/install/install-comfyui)

## Manejo de modelos faltantes
ComfyUI detectará automáticamente los modelos faltantes al cargar flujos:
![Aviso de modelos faltantes](/readme_images/missing_models.png)

### Para usuarios de ComfyUI Desktop
1. Haga clic en el botón de descarga en el popup
2. Notas:
   - Actualmente solo soporta modelos de CivitAI y Hugging Face
   - Asegure la conectividad a estas plataformas
   - Formatos no soportados (.pth) se documentan en readme.md para descarga manual

### Otras versiones

1. Haga clic en `Download` para iniciar descarga, luego mueva manualmente a `ComfyUI/models/`

Estructura de directorios:
```bash
ComfyUI/
└── models/
    ├── checkpoints/
    │   └── dreamshaper_8.safetensors
    └── loras/
        ├── blindbox_ViMix.safetensors
        └── MoXinV1.safetensors
```
> Reinicie/actualice la interfaz después de mover archivos

## Manejo de nodos faltantes
![Aviso de nodos faltantes](/readme_images/missing_node_types.png)

### Soluciones
1. **Nodos principales faltantes**: [Actualice ComfyUI](https://comfyui-wiki.com/es/tutorial/basic/how-to-update-comfyui)
2. **Nodos personalizados faltantes**: Instale mediante ComfyUI Manager

### Guía de instalación con ComfyUI Manager
![Interfaz de ComfyUI Manager](/readme_images/comfyui_manager.png)
1. Haga clic en `Manager`
2. Seleccione `Install missing nodes`
3. Haga clic en `Install` en el popup

![Ejemplo de instalación](/readme_images/install_missing_nodes.jpg)

### Notas importantes
- Requiere acceso a GitHub para instalación automática
- Usuarios con restricciones consulten [guía de instalación manual](https://comfyui-wiki.com/es/install/install-custom-nodes)
- Los README de cada flujo contienen URLs de nodos personalizados

by [@ComfyUI-Wiki](https://github.com/comfyui-wiki) | [ComfyUI-Wiki](https://comfyui-wiki.com/es)