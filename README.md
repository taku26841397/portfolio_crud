# 📚 本棚アプリ（Django CRUD / ポートフォリオ作品）

自分が読了した本を管理するために作成した Django 製の本棚アプリです。  
タイトル・著者・ジャンル・感想などを登録し、一覧・詳細・編集・削除ができる CRUD アプリケーションです。  
ログイン機能を備え、認証済みユーザーのみが本棚を操作できるようにしています。

---

## 🌐 公開 URL
https://（あなたのRenderのURL）

---

## 🔑 テストユーザー（企業向け）
動作確認用のユーザーを用意しています。

- ユーザー名：testuser  
- パスワード：testpass123  

---

## 🛠 使用技術
- Python 3.14.4
- Django 6.0.4 
- Bootstrap 5  
- Render（デプロイ）  
- SQLite（開発環境）  

---

## 📌 機能一覧
- 本の登録（タイトル / 著者 / ジャンル / 読了日 / 感想）
- 一覧表示（ListView）
- 詳細表示（DetailView）
- 編集（UpdateView）
- 削除（DeleteView）
- ログイン / ログアウト機能
- LoginRequiredMixin によるアクセス制御
- 画像アップロード（本の表紙）
- ページネーション

---

## 🎨 UI / デザインのポイント
- Bootstrap を使用し、デザインをシンプルかつ読みやすく  
- 本の一覧をカード形式で表示し、視認性を向上  
- UIをCRUD操作を直感的に行えるよう調整 
- ログイン機能 

---

## 🧩 工夫した点
- Django のクラスベースビュー（CBV）を活用し、コードの簡潔さと拡張性を重視  
- LoginRequiredMixin によるセキュリティ確保  
- Render へのデプロイを通じて、本番環境での動作を確認  
- DB に testuser を作成 
- 実際に読了した本を登録することで、アプリの使用イメージが伝わりやすい構成にした  

---

## 📁 ディレクトリ構成（抜粋）

- crud/　：本棚アプリのメイン機能（モデル・ビュー・テンプレート）
- media_local/　：アップロードした本の表紙画像を保存
- myproject/　：Django プロジェクト設定（settings.py など）
- manage.py　：Django の起動スクリプト
- requirements.txt　：使用パッケージ一覧
- Procfile　：Render デプロイ用設定

- ## 📁 crud アプリの構成

crud/
  - migrations/        ← DB マイグレーション
  - templates/         ← HTML テンプレート
  - admin.py           ← 管理画面の設定
  - apps.py            ← アプリ設定
  - models.py          ← 本のデータモデル
  - views.py           ← CRUD の処理（一覧・詳細・作成・編集・削除）
  - urls.py            ← アプリ内の URL ルーティング
  - tests.py           ← テスト（未使用）
  - __init__.py



---

## 📄 ライセンス
このプロジェクトは学習目的で作成したものです。

