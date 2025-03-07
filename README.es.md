# Flujos de trabajo de ComfyUI Wiki
🌐 Soporte multilingüe: [English](README.md) | [中文](README.zh.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

Este repositorio almacena todos los archivos de flujo de trabajo para [ComfyUI-Wiki.com](https://comfyui-wiki.com/es). Cada flujo incluye una imagen de vista previa (con metadatos incrustados) y un archivo JSON. Ambos formatos se pueden arrastrar directamente a ComfyUI para cargarlos.

## Primeros pasos

### Requisitos previos
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) instalado
- Para nuevas instalaciones, siga la [Guía de instalación de ComfyUI Wiki](https://comfyui-wiki.com/es/install/install-comfyui)

## Manejo de modelos faltantes
Al cargar flujos de trabajo, ComfyUI detectará automáticamente y solicitará los modelos faltantes:
![Aviso de modelos faltantes](/readme_images/missing_models.png)

### Para usuarios de ComfyUI Desktop
1. Haga clic en el botón de descarga en el cuadro de diálogo
2. Notas importantes:
   - Solo admite modelos de [CivitAI](https://civitai.com) y [Hugging Face](https://huggingface.co/)
   - Asegúrese de tener acceso a estas plataformas
   - Los tipos de archivo no compatibles (por ejemplo, .pth) tendrán instrucciones separadas

### Para otras versiones (Portátiles/Instalaciones manuales)
1. Los archivos descargados se guardarán en su navegador
2. Mueva manualmente los archivos a los subdirectorios correspondientes en `ComfyUI/models/`

Ejemplo de estructura después de la configuración:
```bash
ComfyUI/
└── models/
    ├── checkpoints/
    │   └── dreamshaper_8.safetensors
    └── loras/
        ├── blindbox_ViMix.safetensors
        └── MoXinV1.safetensors
```
> Reinicie/actualice ComfyUI después de mover los archivos

## Resolución de nodos faltantes
![Aviso de nodos faltantes](/readme_images/missing_node_types.png)

### Pasos para solucionar problemas
1. **Faltan nodos principales**: [Actualice ComfyUI](https://comfyui-wiki.com/es/tutorial/basic/how-to-update-comfyui)
2. **Faltan nodos personalizados**: Instale a través de ComfyUI Manager

### Guía de instalación
![Interfaz de ComfyUI Manager](/readme_images/comfyui_manager.png)
1. Haga clic en el botón `Manager` en ComfyUI
2. Seleccione `Install missing nodes`
3. Haga clic en `Install` en el cuadro de diálogo

![Demostración de instalación de nodos](/readme_images/install_missing_nodes.jpg)

### Notas importantes
- Requiere acceso a GitHub para instalaciones automáticas
- Guía de instalación manual disponible para redes restringidas: [Instalación de nodos personalizados](https://comfyui-wiki.com/es/install/install-custom-nodes)
- La información específica de los nodos se proporciona en los archivos README individuales

> Todos los flujos de trabajo pasan controles de seguridad. Obtenga modelos solo de fuentes oficiales. 