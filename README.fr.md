# Workflows ComfyUI Wiki
🌐 Support multilingue : [English](README.md) | [中文](README.zh.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

Ce dépôt contient tous les workflows pour [ComfyUI-Wiki.com](https://comfyui-wiki.com/fr). Chaque workflow inclut une image prévisualisable (avec métadonnées) et un fichier JSON.

## Premiers pas

### Prérequis
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) installé
- Suivez le [Guide d'installation de ComfyUI Wiki](https://comfyui-wiki.com/fr/install/install-comfyui) pour les nouvelles installations

## Gestion des modèles manquants
![Alerte modèles manquants](/readme_images/missing_models.png)

### Pour ComfyUI Desktop
1. Cliquez sur le bouton de téléchargement
2. Notes importantes :
   - Modèles uniquement de CivitAI et Hugging Face
   - Formats .pth non supportés
   - Assurez-vous de l'accès réseau

### Autres versions
1. Déplacez les fichiers dans `ComfyUI/models/`

Structure exemple :
```bash
ComfyUI/
└── models/
    ├── checkpoints/
    │   └── dreamshaper_8.safetensors
    └── loras/
        ├── blindbox_ViMix.safetensors
        └── MoXinV1.safetensors
```
> Redémarrez/rafraîchissez ComfyUI après déplacement

## Résolution des nœuds manquants
![Alerte nœuds manquants](/readme_images/missing_node_types.png)

### Dépannage
1. **Nœuds principaux manquants** : [Mettre à jour ComfyUI](https://comfyui-wiki.com/fr/tutorial/basic/how-to-update-comfyui)
2. **Nœuds personnalisés manquants** : Installer via ComfyUI Manager

### Guide d'installation
![Interface ComfyUI Manager](/readme_images/comfyui_manger.png)
1. Cliquez sur le bouton `Manager`
2. Sélectionnez `Install missing nodes`
3. Cliquez sur `Install`

![Démonstration d'installation](/readme_images/install_missing_nodes.jpg)

### Notes importantes
- Nécessite l'accès à GitHub pour l'installation automatique
- Guide d'installation manuelle : [Installation de nœuds personnalisés](https://comfyui-wiki.com/fr/install/install-custom-nodes)
- Informations spécifiques dans chaque README de workflow

> Tous les workflows sont vérifiés pour la sécurité. Utilisez des modèles officiels 