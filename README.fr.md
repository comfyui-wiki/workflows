# Workflows ComfyUI Wiki
🌐 Support multilingue : [English](README.md) | [中文](README.zh.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

Ce dépôt contient tous les fichiers de workflow du site [ComfyUI-Wiki.com](https://comfyui-wiki.com/fr). Chaque workflow inclut une prévisualisation (avec métadonnées) et un fichier JSON, utilisables par glisser-déposer dans ComfyUI.

## Premiers pas

Après avoir téléchargé les modèles correspondants, faites-les glisser dans ComfyUI pour charger le workflow associé. Chaque fichier de workflow contient un readme.md avec les informations de téléchargement.

### Prérequis
- Installation de [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
- Nouveaux utilisateurs : consultez le [guide d'installation ComfyUI Wiki](https://comfyui-wiki.com/fr/install/install-comfyui)

## Gestion des modèles manquants
ComfyUI détecte automatiquement les modèles absents lors du chargement d'un workflow :
![Alerte modèles manquants](/readme_images/missing_models.png)

### Utilisateurs de la version desktop
1. Cliquez sur le bouton de téléchargement dans la fenêtre pop-up
2. Notes importantes :
   - Seuls les modèles de CivitAI et Hugging Face sont actuellement détectés
   - Vérifiez votre connexion à ces plateformes
   - Les formats non supportés (.pth etc.) sont documentés dans le readme.md pour téléchargement manuel

### Autres versions

1. Cliquez `Download` pour lancer le téléchargement via navigateur, puis déplacez manuellement le fichier dans `ComfyUI/models/`

Structure d'exemple :
```bash
ComfyUI/
└── models/
    ├── checkpoints/
    │   └── dreamshaper_8.safetensors
    └── loras/
        ├── blindbox_ViMix.safetensors
        └── MoXinV1.safetensors
```
> Redémarrez/rafraîchissez l'interface après déplacement

## Gestion des nœuds manquants
![Alerte nœuds manquants](/readme_images/missing_node_types.png)

### Solutions
1. **Nœuds principaux manquants** : [Mettez à jour ComfyUI](https://comfyui-wiki.com/fr/tutorial/basic/how-to-update-comfyui)
2. **Nœuds personnalisés manquants** : Installation via ComfyUI Manager

### Guide d'installation avec ComfyUI Manager
![Interface ComfyUI Manager](/readme_images/comfyui_manager.png)
1. Cliquez `Manager`
2. Sélectionnez `Install missing nodes`
3. Cliquez `Install` dans la fenêtre pop-up

![Exemple d'installation](/readme_images/install_missing_nodes.jpg)

### Informations importantes
- L'installation automatique nécessite un accès à GitHub
- Utilisateurs avec restrictions réseau : consultez le [guide d'installation manuelle](https://comfyui-wiki.com/fr/install/install-custom-nodes)
- Les README des workflows contiennent les URLs des nœuds personnalisés

par [@ComfyUI-Wiki](https://github.com/comfyui-wiki) | [ComfyUI-Wiki](https://comfyui-wiki.com/fr)