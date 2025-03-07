# ComfyUI Wiki ワークフロー
🌐 多言語対応: [English](README.md) | [中文](README.zh.md) | [Español](README.es.md) | [Français](README.fr.md) | [한국어](README.ko.md)

このリポジトリは[ComfyUI-Wiki.com](https://comfyui-wiki.com/ja)の全ワークフローファイルを保管しています。各ワークフローにはプレビュー画像（メタデータ埋め込み）とJSONファイルが含まれており、どちらもComfyUIに直接ドラッグして読み込むことが可能です。

## セットアップ

対応するモデルをダウンロード後、ComfyUIにドラッグして対応するワークフローを読み込むことができます。各ワークフローファイルには、関連モデルのダウンロード情報を記載したreadme.mdが含まれています。

### 環境要件
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) がインストール済み
- 新規ユーザーは[ComfyUI Wikiインストールガイド](https://comfyui-wiki.com/ja/install/install-comfyui)を参照してください

## 不足モデルの対応
ワークフロー読み込み時、ComfyUIは自動的に不足モデルを検出します：
![不足モデル通知](/readme_images/missing_models.png)

### ComfyUI Desktopユーザー
1. 通知ダイアログのダウンロードボタンをクリック
2. 重要事項：
   - 現在CivitAIとHugging Faceのモデルのみ対応
   - 各プラットフォームへのネットワーク接続を確認
   - .pth形式など非対応ファイルはreadme.mdに手動手順を記載

### その他バージョン
1. `Download`ボタンでブラウザからファイルをダウンロード
2. ダウンロード完了後、手動で`ComfyUI/models/`に移動

ディレクトリ構造例：
```bash
ComfyUI/
└── models/
    ├── checkpoints/
    │   └── dreamshaper_8.safetensors
    └── loras/
        ├── blindbox_ViMix.safetensors
        └── MoXinV1.safetensors
```
> ファイル移動後、ComfyUIを再起動/リフレッシュしてください

## 不足ノードの解決
![不足ノード通知](/readme_images/missing_node_types.png)

### 解決方法
1. **コアノード不足**: [ComfyUIの更新](https://comfyui-wiki.com/ja/tutorial/basic/how-to-update-comfyui)
2. **カスタムノード不足**: ComfyUI Managerでインストール

### ComfyUI Manager操作手順
![ComfyUI Manager画面](/readme_images/comfyui_manager.png)
1. `Manager`ボタンをクリック
2. `Install missing nodes`を選択
3. ポップアップで`Install`をクリック

![ノードインストール例](/readme_images/install_missing_nodes.jpg)

### 重要注意事項
- 自動インストールにはGitHubへのアクセスが必要
- ネットワーク制限環境の場合は[手動インストールガイド](https://comfyui-wiki.com/ja/install/install-custom-nodes)を参照
- 各ワークフローのREADMEにカスタムノードURLを記載

by [@ComfyUI-Wiki](https://github.com/comfyui-wiki) | [ComfyUI-Wiki](https://comfyui-wiki.com/ja)