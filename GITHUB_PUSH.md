# GitHub へのプッシュ手順

## 1. GitHubで新規リポジトリを作成

1. [GitHub](https://github.com)にログイン
2. 右上の「+」→「New repository」をクリック
3. リポジトリ名を入力（例: `eraser-battle-arena`）
4. 「Public」または「Private」を選択
5. **「Initialize this repository with a README」はチェックしない**
6. 「Create repository」をクリック

## 2. ローカルでGitリポジトリを初期化

```bash
cd eraser-battle-arena
git init
git add .
git commit -m "Initial commit: Eraser Battle Arena game"
```

## 3. GitHubリポジトリと接続

GitHubで作成したリポジトリのURLを使用します（例: `https://github.com/yourusername/eraser-battle-arena.git`）

```bash
git remote add origin https://github.com/yourusername/eraser-battle-arena.git
git branch -M main
git push -u origin main
```

## 4. 以降の更新手順

ファイルを変更した後:

```bash
git add .
git commit -m "変更内容の説明"
git push
```

## 📊 プロジェクト統計

- **総ファイル数**: 約 80ファイル（不要なUIコンポーネントを削除済み）
- **プロジェクトサイズ**: 約 5.9MB
- **使用UIコンポーネント**: 12個のみ（必要最小限）

## ⚡ 最適化済み

このプロジェクトは以下の最適化が施されています:

- ✅ 不要なUIコンポーネント35個を削除
- ✅ .gitignoreファイルを整備
- ✅ node_modules, dist, .localなど不要なファイルを除外
- ✅ README.mdを追加

## 🔧 トラブルシューティング

### Git認証エラーが出る場合

HTTPSでプッシュする際に認証エラーが出る場合は、Personal Access Tokenを使用してください:

1. GitHub Settings → Developer settings → Personal access tokens → Tokens (classic)
2. 「Generate new token」をクリック
3. `repo`のスコープを選択
4. トークンを生成してコピー
5. Gitのパスワード入力時にこのトークンを使用

### SSHを使用する場合

```bash
git remote set-url origin git@github.com:yourusername/eraser-battle-arena.git
```

事前にSSHキーをGitHubに登録する必要があります。
