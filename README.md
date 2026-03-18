# Eraser Battle Arena

消しゴムバトルアリーナゲーム - カスタム消しゴムでバトルを楽しもう!

## 🎮 特徴

- **カスタム消しゴム作成**: 自分だけのオリジナル消しゴムをデザイン
- **リアルタイムバトル**: 物理演算を使用した本格的なバトル体験
- **多様な戦略**: 重さ、弾力性、摩擦などのパラメータを調整して最適な戦略を構築

## 🚀 セットアップ

### 必要要件

- Node.js 18以上
- npm または yarn

### インストール

```bash
# 依存関係をインストール
npm install

# 開発サーバーを起動
npm run dev
```

### ビルド

```bash
# プロダクションビルド
npm run build

# プレビュー
npm run preview
```

## 🛠️ 技術スタック

- **フロントエンド**: React, TypeScript, Vite
- **スタイリング**: Tailwind CSS, shadcn/ui
- **バックエンド**: Express, TypeScript
- **データベース**: Drizzle ORM
- **状態管理**: Zustand
- **物理演算**: カスタム実装

## 📁 プロジェクト構造

```
eraser-battle-arena/
├── client/          # フロントエンドコード
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   └── lib/
│   └── index.html
├── server/          # バックエンドコード
│   ├── routes.ts
│   ├── db.ts
│   └── storage.ts
├── shared/          # 共有型定義
└── script/          # ビルドスクリプト
```

## 🎯 ゲームのルール

1. 消しゴムのパラメータを設定
2. バトルアリーナに配置
3. 物理演算によるリアルタイムバトル
4. 最後まで残った消しゴムが勝者!

## 📝 ライセンス

MIT License

## 🤝 コントリビューション

プルリクエストを歓迎します。大きな変更の場合は、まずissueを開いて変更内容を議論してください。
