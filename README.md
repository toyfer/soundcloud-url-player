# 🎵 SoundCloud Player

モバイル最適化されたSoundCloudプレイヤー。公式パラメータのみを使用し、より安定した再生体験を提供します。

## ✨ 特徴

- **モバイルファースト設計**: タッチ操作とモバイル画面に最適化
- **公式APIのみ使用**: 長期的な安定性を確保
- **PWA対応**: ホーム画面に追加してアプリのように使用可能
- **シンプルなUI**: 余計な要素を排除したクリーンなデザイン

## 🚀 使用方法

### 基本的な使用方法
1. SoundCloud URLを入力フィールドに貼り付け
2. 「読み込み」ボタンをクリック
3. 楽曲が再生されます

### URLパラメータでの直接アクセス
```
https://[ユーザー名].github.io/soundcloud-player/?url=https://soundcloud.com/artist/track-name
```

### PWA（アプリ化）
- 対応ブラウザで「ホーム画面に追加」ボタンが表示されます
- ホーム画面に追加するとアプリのように起動できます

## 🔧 技術的特徴

### Phase 1: 公式パラメータ移行（完了）
- ❌ 非公式パラメータを削除: `hide_related`, `show_comments`, `show_reposts`, `show_teaser`, `visual`
- ✅ 公式パラメータのみ使用: `url`, `auto_play`, `buying`, `sharing`, `download`, `show_artwork`, `show_playcount`, `show_user`, `single_active`, `color`
- ✅ SoundCloud Widget API統合
- ✅ エラーハンドリング強化

### Phase 2: PWA機能（完了）
- ✅ Service Worker実装
- ✅ Web App Manifest
- ✅ インストール促進UI
- ✅ オフライン対応

### モバイル最適化
- ✅ タッチイベント最適化
- ✅ 画面回転対応
- ✅ レスポンシブデザイン

## 📱 対応環境
- iOS Safari
- Android Chrome
- デスクトップブラウザ全般

## 🛠️ 開発者向け

このプロジェクトは単一のHTMLファイルで構成されており、追加の依存関係はありません。

### ローカル開発
```bash
python3 -m http.server 8000
```

### デプロイ
静的ファイルホスティングサービス（GitHub Pages、Netlify、Vercel等）にそのままアップロード可能です。