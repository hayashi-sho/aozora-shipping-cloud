# AOZORA. Shipping Cloud v0.3 (MUNBYN ITPP130B / iPhone)

## 内容
- `index.html`: GitHub Pagesで公開可能な単一HTMLファイル（Amazon注文→クリックポストCSV、クリックポスト正式発行PDF→MUNBYN用4x6インチPDF）
- `AOZORA_Shipping_Cloud_MUNBYN_iPhone_操作説明書_v0.3.pdf`: 手順書

## GitHub Pagesへの登録
GitHubでリポジトリ作成→`index.html`アップロード→Settings→Pages→main/(root)。公開後はSafariで開いてホーム画面へ追加。

## PDF変換の仕様と制限
- PDF形式はA4の4面(左右上下の均等4分割)、A4左上1面、A6全面1面。出力は4x6インチ(101.6x152.4mm)の1件1ページ。
- PDFページはベクターを保持したまま切り出します。回転・空白枠スキップを指定可能ですが、自動ラベル検知は非対応。
- PDF処理に `pdf-lib@1.17.1` をCDNから読み込むため、初回・通常ともネット接続が必要です。データはブラウザー内で処理し、外部APIへアップロードしません。
- GitHub Pagesで公開するファイルは`index.html`のみ。注文ファイル、PDF、住所をアップロードしないこと。
- プリンターへの直接Bluetooth印刷ではなく、Munbyn Print公式アプリへPDFを渡して印刷します。
- 未検証：iPhone実機／クリックポスト実データ／ITPP130B実機でのエンドツーエンド動作。

## 重要
ラベル印刷前に必ず宛名、枚数、コードの欠けと読取、縮尺、向きを照合してください。クリックポストの申込・決済・送り状発行・Amazon発送通知は手動です。
