# 休養インストラクター 佐々木知広 - ランディングページ

## 📋 概要
このランディングページは、休養インストラクター 佐々木知広様の講座案内および問い合わせ窓口として作成されました。

## 📁 ファイル構成
```
landing-page/
├── index.html          # メインHTMLファイル
├── style.css           # スタイルシート
└── README.md           # このファイル
```

## 🌟 主な機能

### 掲載内容
1. **ヒーローセクション**
   - キャッチコピー：「正しく休めば、パフォーマンスは劇的に変わる」
   - 資格バッジ（NHK出演、ZPP認定、柔道整復師等）

2. **プロフィールセクション**
   - 詳細な経歴・資格情報
   - NHK出演実績
   - 専門分野の紹介
   - Instagramリンク

3. **講座内容セクション**
   - 教育機関向け
   - 企業向け
   - 自治体・地域向け
   - 個人向け

4. **実績セクション**
   - メディア出演
   - 教育機関での実績
   - 商業施設での講座
   - 地域イベント
   - 個人・小規模講座

5. **お問い合わせセクション**
   - メールアドレス
   - Instagram QRコード
   - Googleフォームへのリンク

## 🚀 GitHub Pagesでの公開手順

### Step 1: GitHubアカウントの作成（お持ちでない場合）
1. https://github.com にアクセス
2. 「Sign up」をクリック
3. メールアドレス、パスワードを設定
4. アカウント作成完了

### Step 2: リポジトリの作成
1. GitHubにログイン
2. 右上の「+」→「New repository」をクリック
3. 以下のように設定：
   - **Repository name**: `kyuyo-instructor`（または任意の名前）
   - **Public**を選択（無料でPages使用のため）
   - 「Create repository」をクリック

### Step 3: ファイルのアップロード

#### 方法A: Webインターフェースから（簡単）
1. 作成したリポジトリのページで「uploading an existing file」をクリック
2. `index.html`と`style.css`を選択してドラッグ&ドロップ
3. 下部の「Commit changes」をクリック

#### 方法B: Gitコマンドから（技術的）
```bash
# ローカルにクローン
git clone https://github.com/あなたのユーザー名/kyuyo-instructor.git
cd kyuyo-instructor

# ファイルをコピー
# index.htmlとstyle.cssをこのフォルダに配置

# コミット＆プッシュ
git add .
git commit -m "Initial commit: Landing page"
git push origin main
```

### Step 4: GitHub Pagesの有効化
1. リポジトリのページで「Settings」タブをクリック
2. 左メニューから「Pages」を選択
3. **Source**セクションで：
   - Branch: `main`を選択
   - Folder: `/ (root)`を選択
4. 「Save」をクリック
5. 数分待つと、ページが公開されます

### Step 5: 公開URLの確認
- 公開URL：`https://あなたのユーザー名.github.io/kyuyo-instructor/`
- このURLをブラウザで開いて確認

## ⚙️ 公開後の設定

### Googleフォームの設定と連携

1. **Googleフォームの作成**
   - https://forms.google.com にアクセス
   - 「空白」から新規フォームを作成
   - 以下の項目を追加：
     ```
     - お名前（短答記述式・必須）
     - メールアドレス（短答記述式・必須）
     - 電話番号（短答記述式・任意）
     - 所属（短答記述式・任意）
     - お問い合わせ内容（プルダウン・必須）
       選択肢：講座依頼 / 見積もり希望 / その他
     - 希望の講座内容（段落記述式・任意）
     - 希望日時（段落記述式・任意）
     - メッセージ（段落記述式・任意）
     ```

2. **フォームの公開**
   - 右上の「送信」をクリック
   - リンクタブを選択
   - 「URLを短縮」にチェック
   - リンクをコピー（例：`https://forms.gle/xxxxx`）

3. **HTMLへのリンク追加**
   - `index.html`の234行目付近を編集：
   ```html
   <a href="あなたのGoogleフォームURL" target="_blank" class="form-button">
   ```
   - 編集後、再度GitHubにアップロード

### LINE公式アカウント追加（オプション）
LINEでの問い合わせも受け付けたい場合：
1. LINE公式アカウントを作成
2. QRコードを取得
3. お問い合わせセクションに追加

## 🔧 カスタマイズ方法

### 色の変更
`style.css`の6-12行目を編集：
```css
:root {
    --primary-color: #2c3e50;      /* メインカラー */
    --secondary-color: #34495e;    /* サブカラー */
    --accent-color: #3498db;       /* アクセントカラー */
}
```

### 写真の変更
- プロフィール写真などを差し替えたい場合
- 画像をどこかにアップロード（Imgur、Googleドライブ等）
- `index.html`内の画像URLを変更

### テキストの修正
- `index.html`を直接編集
- GitHubの「Code」タブ → ファイルをクリック → 鉛筆アイコンで編集可能

## 📱 レスポンシブ対応
- スマートフォン、タブレット、PCすべてに対応
- 自動的にデバイスサイズに合わせて表示が調整されます

## 🔍 SEO対策済み
- メタディスクリプション設定済み
- 適切な見出しタグ構造
- 画像にalt属性設定

## 📊 アクセス解析の追加（推奨）
Google Analyticsを追加する場合：
1. Google Analyticsでアカウント作成
2. トラッキングコードを取得
3. `index.html`の`</head>`タグの前に挿入

## 🆘 トラブルシューティング

### ページが表示されない
- GitHub Pagesの設定を確認
- ファイル名が`index.html`になっているか確認
- ブラウザのキャッシュをクリア

### デザインが崩れる
- `style.css`が正しくアップロードされているか確認
- ファイル名のスペルミスがないか確認

### 画像が表示されない
- 画像URLが正しいか確認
- 画像ファイルが公開状態か確認

## 📞 サポート
不明点があれば、以下をご確認ください：
- GitHub Pages公式ドキュメント: https://pages.github.com/
- Googleフォームヘルプ: https://support.google.com/forms/

## ✅ 公開前チェックリスト
- [ ] index.htmlとstyle.cssをGitHubにアップロード
- [ ] GitHub Pagesを有効化
- [ ] 公開URLでページが表示されることを確認
- [ ] Googleフォームを作成
- [ ] フォームのリンクをHTMLに追加
- [ ] スマートフォンで表示確認
- [ ] すべてのリンクが正しく動作するか確認
- [ ] メールアドレスが正しいか確認
- [ ] InstagramのQRコードが正しいか確認

## 🎉 完成後
公開URLを以下の場所で活用してください：
- 名刺にQRコードで掲載
- メール署名に追加
- SNSプロフィールにリンク
- パンフレットに記載

---

**作成日**: 2026年2月2日  
**対象**: 休養インストラクター 佐々木知広様  
**月額費用**: 完全無料（GitHub Pages使用）