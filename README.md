# social-pulse

![SocialPulse Screenshot](https://via.placeholder.com/1000x500.png?text=SocialPulse+Screenshot+Placeholder)

## 概要 / Overview

**SocialPulse** は、高度な条件設定に基づいて架空のSNS（ツイート）データを検索・抽出・分析するAI駆動のシングルページアプリケーション（SPA）です。Gemini APIを活用し、特定のターゲット層や条件に合致するツイート群をシミュレートして生成するほか、抽出したデータに対するAI要約・感情分析を行うことができます。マーケティングリサーチのシミュレーションや、ペルソナ分析のためのデータ作成などに最適です。

**SocialPulse** is an AI-driven Single Page Application (SPA) for searching, extracting, and analyzing simulated social media (tweet) data based on advanced condition settings. Leveraging the Gemini API, it generates simulated tweets matching specific target demographics and conditions, and performs AI-based summarization and sentiment analysis on the extracted data. It is ideal for marketing research simulations and generating data for persona analysis.

---

## 主な機能一覧 / Features

- **AIによる検索条件の自動提案 (AI Setup)**
  テーマを入力するだけで、AIがターゲット層やメタデータ条件（エンゲージメント数など）を自動構成します。
- **高度なカスタマイズ (Advanced Customization)**
  ユーザー属性、期間、除外ルール（Botアカウントの除外など）を細かく手動設定可能です。
- **データ抽出・出力 (Data Extraction & Output)**
  抽出したデータを「リスト表示」または「CSV形式」で出力・生成します。
- **ワンクリックコピー (One-Click Copy)**
  抽出したデータをワンクリックでクリップボードにコピーできます。
- **AIインサイト分析 (AI Insight Analysis)**
  抽出したデータに対して、AIが要約、頻出キーワードの抽出、感情分析（ポジティブ/ネガティブ/中立）を即座に実行します。
- **ローカルセーブ機能 (Local Save)**
  入力したAPIキーや設定条件はブラウザのローカルストレージに自動保存され、次回利用時にも引き継がれます。

- **AI-Powered Condition Setup**: Simply enter a theme, and the AI will automatically suggest target demographics and metadata conditions (e.g., engagement metrics).
- **Advanced Customization**: Finely tune settings manually, including user attributes, time periods, and exclusion rules (e.g., ignoring bot accounts).
- **Data Extraction & Output**: Output generated data in "List" or "CSV" formats.
- **One-Click Copy**: Copy the extracted data to your clipboard with a single click.
- **AI Insight Analysis**: The AI instantly performs summarization, keyword extraction, and sentiment analysis (positive/negative/neutral) on the extracted data.
- **Local Save**: Your API key and configured settings are automatically saved in the browser's LocalStorage for future sessions.

---

## 使用技術・ライブラリ / Technologies & Libraries

- **Frontend**: HTML5, JavaScript (Vanilla JS), CSS3
- **Styling**: Tailwind CSS (via CDN)
- **Backend/API**: Cloudflare Workers (as a proxy endpoint), Google Gemini API
- **Storage**: Browser LocalStorage

---

## セットアップ・使い方 / Setup & Usage

### セットアップ / Setup

1. このリポジトリの `index.html` ファイルをダウンロード、またはリポジトリをクローンします。
2. ダウンロードした `index.html` をお好みのWebブラウザで開きます（Node.jsなどの特別なローカルサーバー環境は不要です）。
3. 画面右上の入力欄に、ご自身の **Gemini API Key** を入力します。

1. Download the `index.html` file from this repository or clone the repository.
2. Open `index.html` in your preferred web browser. (No specific local server environment like Node.js is required.)
3. Enter your **Gemini API Key** in the input field located at the top right of the screen.

### 使い方 / Usage

1. **条件の構成 (オプション) / Configure Conditions (Optional)**:
   - 「🎯 高度な検索・ターゲット条件」のセクションを開きます。
   - 「AIに検索条件を提案させる」の欄にテーマ（例：最新のAIツール）を入力し、「構成開始」をクリックすると、AIが自動で最適な条件を入力します。手動での書き換えも可能です。
2. **データの検索と抽出 / Search and Extract Data**:
   - 「🔍 ツイートを検索・抽出する」セクションで、出力形式（リスト表示またはCSV形式）を選択します。
   - 検索キーワードやハッシュタグを入力し、「SEARCH & EXTRACT」ボタンをクリックします。
3. **結果の分析とコピー / Analyze and Copy Results**:
   - 画面下部に結果が出力されます。
   - 「COPY TO CLIPBOARD」ボタンで抽出したデータをコピーできます。
   - 「AI ANALYSIS (要約・感情)」ボタンをクリックすると、抽出データに基づいたインサイト（要約と感情分析結果）が追加で表示されます。

1. **Configure Conditions (Optional)**:
   - Expand the "🎯 高度な検索・ターゲット条件" (Advanced Search & Target Conditions) section.
   - Enter a theme (e.g., "Latest AI tools") and click "構成開始" (Start Setup). The AI will automatically fill in the optimal conditions. You can also manually edit these fields.
2. **Search and Extract Data**:
   - In the "🔍 ツイートを検索・抽出する" (Search & Extract Tweets) section, select your desired output format (List or CSV).
   - Enter your search keywords or hashtags, then click the "SEARCH & EXTRACT" button.
3. **Analyze and Copy Results**:
   - The results will be displayed at the bottom of the screen.
   - Click "COPY TO CLIPBOARD" to easily copy the generated text.
   - Click "AI ANALYSIS (要約・感情)" to reveal AI-generated insights, including a summary and sentiment analysis based on the extracted data.

---

## ライセンス / License

このプロジェクトは **MIT License** のもとで公開されています。自由に複製、変更、配布することが可能です。

This project is licensed under the **MIT License**. You are free to use, modify, and distribute it.