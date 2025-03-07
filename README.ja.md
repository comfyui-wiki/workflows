# ComfyUI Wiki ワークフロー
🌐 多言語対応: [English](README.md) | [中文](README.zh.md) | [Español](README.es.md) | [Français](README.fr.md) | [한국어](README.ko.md)

このリポジトリは[ComfyUI-Wiki.com](https://comfyui-wiki.com/ja)の全ワークフローファイルを保管しています。各ワークフローにはプレビュー画像（メタデータ埋め込み）とJSONファイルが含まれており、どちらもComfyUIに直接ドラッグして読み込むことが可能です。

## セットアップ

### 必要条件
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) がインストール済み
- 新規インストールの場合は[ComfyUI Wikiインストールガイド](https://comfyui-wiki.com/ja/install/install-comfyui)に従ってください

## 不足モデルの対応
ワークフロー読み込み時、ComfyUIは自動的に不足モデルを検出し通知します：
![不足モデル通知](/readme_images/missing_models.png)

### ComfyUI Desktopユーザー
1. 通知ダイアログのダウンロードボタンをクリック
2. 重要事項：
   - [CivitAI](https://civitai.com)と[Hugging Face](https://huggingface.co/)のモデルのみ対応
   - 各プラットフォームへのネットワーク接続を確認
   - 非対応ファイル形式（例：.pth）は別途案内あり

### その他バージョン（ポータブル/手動インストール）
1. ブラウザに保存されたダウンロードファイルを確認
2. `ComfyUI/models/`の適切なサブディレクトリに手動で移動

設定後のディレクトリ例：
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

### トラブルシューティング手順
1. **コアノード不足**: [ComfyUIの更新](https://comfyui-wiki.com/ja/tutorial/basic/how-to-update-comfyui)
2. **カスタムノード不足**: ComfyUI Manager経由でインストール

### インストールガイド
![ComfyUI Managerインターフェース](/readme_images/comfyui_manager.png)
1. ComfyUIの`Manager`ボタンをクリック
2. `Install missing nodes`を選択
3. ダイアログで`Install`をクリック

![ノードインストールデモ](/readme_images/install_missing_nodes.jpg)

### 重要事項
- 自動インストールにはGitHubへのアクセスが必要
- 制限ネットワーク環境向け手動インストールガイド: [カスタムノードのインストール](https://comfyui-wiki.com/ja/install/install-custom-nodes)
- 各ワークフロー固有のノード情報は個別READMEファイルに記載

> 全ワークフローはセキュリティチェックを通過しています。モデルは公式ソースからのみ入手してください。 