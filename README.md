# 🚗 Car Manager

車両管理PWAアプリ — 燃費・給油・メンテナンス・車検・走行距離を一元管理

## 📁 ファイル構成

```
carmanager/
├── index.html          # アプリ本体
├── manifest.json       # PWA設定
├── sw.js               # Service Worker（オフライン対応）
├── favicon.ico         # ブラウザタブアイコン
├── apple-touch-icon.png # iOS ホーム画面アイコン
├── icons/              # 各サイズのアイコン
│   ├── icon-72x72.png
│   ├── icon-96x96.png
│   ├── icon-128x128.png
│   ├── icon-144x144.png
│   ├── icon-152x152.png
│   ├── icon-192x192.png
│   ├── icon-256x256.png
│   └── icon-512x512.png
└── README.md
```

## 🚀 GitHub Pages への公開手順

1. GitHubで新しいリポジトリを作成（例: `car-manager`）
2. このフォルダの中身をすべてリポジトリのルートにアップロード
3. リポジトリの **Settings → Pages** を開く
4. Source を **Deploy from a branch** → `main` ブランチ・`/ (root)` を選択して **Save**
5. 数分後に `https://あなたのユーザー名.github.io/car-manager/` で公開される

## 📱 スマホにインストール（PWA）

公開後のURLをスマホで開き：
- **iPhone（Safari）**: 共有ボタン → 「ホーム画面に追加」
- **Android（Chrome）**: メニュー → 「アプリをインストール」または「ホーム画面に追加」

ホーム画面のアイコンからアプリのように起動できます。

## 💾 データについて

- データはブラウザの **localStorage** に自動保存されます
- ブラウザを閉じても次回起動時にデータが復元されます
- オフラインでも動作します（Service Worker によるキャッシュ）
