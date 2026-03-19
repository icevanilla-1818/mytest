# 📦 在庫管理システム

PythonとFlaskを使った、シンプルで使いやすい在庫管理Webアプリケーションです。

## 🌟 特徴

- 🎨 **シンプルで直感的なUI** - 誰でも簡単に使える設計
- 📊 **リアルタイム在庫管理** - 商品の在庫を簡単に追加・削除
- ⚠️ **在庫不足警告** - 在庫が少なくなると自動的に警告表示
- 📱 **レスポンシブデザイン** - パソコン・タブレット・スマートフォン対応
- 🗄️ **SQLiteデータベース** - セットアップ不要で即座に利用可能

## 📋 機能一覧

- ✅ 商品の追加・削除・編集
- ✅ 在庫数の増減管理
- ✅ 商品一覧表示
- ✅ 在庫不足の自動警告
- ✅ 最小在庫数の設定
- ✅ ステータス表示（正常・要注意・在庫不足）

## 🚀 セットアップ

### 必要な環境

- Python 3.7以上
- pip（Pythonパッケージマネージャー）

### インストール手順

1. **リポジトリをクローン**
```bash
git clone https://github.com/icevanilla-1818/mytest.git
cd mytest
```

2. **仮想環境を作成（オプション）**
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

3. **依存パッケージをインストール**
```bash
pip install -r requirements.txt
```

4. **アプリケーションを起動**
```bash
python app.py
```

5. **ブラウザでアクセス**
```
http://localhost:5000
```

## 📖 使い方

### ホーム画面
- システムの概要と登録商品数を確認できます
- 在庫不足商品の数を一目で把握できます

### 商品追加
1. 「➕ 商品追加」ボタンをクリック
2. 商品名、初期在庫数、最小在庫数を入力
3. 「商品を追加」ボタンをクリック

### 在庫管理
1. 「在庫一覧」ページで商品一覧を表示
2. 各商品の右側のボタンで操作：
   - **➕** : 在庫を増やす
   - **➖** : 在庫を減らす
   - **🗑️** : 商品を削除

### 在庫確認
- 各商品のステータスで在庫状況を確認：
  - 🟢 **正常** : 在庫が十分にある
  - 🟡 **要注意** : 在庫が少なくなってきている
  - 🔴 **在庫不足** : 最小在庫数以下（補充推奨）

## 📁 プロジェクト構造

```
mytest/
├── app.py                    # Flaskメインアプリケーション
├── database.py               # データベース処理
├── requirements.txt          # 依存パッケージ
├── inventory.db             # SQLiteデータベース（初回実行時に自動作成）
├── .gitignore               # Git無視ファイル
├── README.md                # このファイル
├── static/
│   └── style.css            # スタイルシート
└── templates/
    ├── base.html            # ベーステンプレート
    ├── index.html           # ホーム画面
    ├── add_product.html     # 商品追加画面
    ├── list_products.html   # 在庫一覧画面
    └── product_detail.html  # 商品詳細画面
```

## 🛠️ 技術スタック

- **Backend**: Flask 2.3.2
- **Database**: SQLite3
- **Frontend**: HTML5, CSS3, JavaScript
- **Python**: 3.7+

## 🔧 トラブルシューティング

### ポート5000が既に使用されている場合
```bash
python app.py --port 5001
```

### データベースをリセットしたい場合
```bash
rm inventory.db
python app.py
```

### 仮想環境から抜ける
```bash
deactivate
```

## 📝 ライセンス

このプロジェクトはMITライセンスの下で公開されています。

## 👨‍💻 開発者

icevanilla-1818

## 🤝 貢献

改善提案やバグ報告は、Issuesで報告してください。

## 📞 サポート

問題が発生した場合は、GitHubのIssuesセクションで報告してください。

---

**楽しい在庫管理を！** 📦✨