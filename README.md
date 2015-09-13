# Web tempates

静的WEBコーディング用テンプレート

## Veriation

* Basic  
基本となるテンプレート
* Bootstrap  
  Bootstrapを基本としたテンプレート

## Detail

### Basic

./basic

#### 対応ブラウザ

IE9+

#### 依存ライブラリ及びフレームワーク

* normalized.css v3.0.2
* jQuery v2.1.4

#### 構成

__js/lib.js__

JavaScriptのライブラリおよび、jQueryプラグインなどを記述するファイル。  
jQueryはデフォルトで含まれている。  
ライブラリ類を別途scriptタグで読み込むと、ローディング時に非効率なため、  
1ファイルにまとめる。

例えばjQueryのスライダープラグインなどはここに追記する。

__js/lib.js__

サイト固有の共通処理を記載する、例えばグローバルメニューのローディングなど。  
ここにはクラスや関数の設定のみを行い、実際に処理を呼び出す際は各ページで行うほうが望ましい。

__img/.gitkeep__

テンプレートをGitで管理する際に必要なだけなので必ず削除する。

__index.html__

* viewport(レスポンシブ)
* SEO対策
  * title
  * description
  * OGPタグ、どこまでやるかは案件により調整する
  * keywordはgoogle,yahooが対応しないため削除
