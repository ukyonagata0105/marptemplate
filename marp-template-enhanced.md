---
marp: true
theme: default
paginate: true
style: |
  section {
    justify-content: start;
    padding: 30px 40px;
    font-size: 1.15em;
  }
  h1 {
    font-size: 1.8em;
    margin-bottom: 0.6em;
    margin-top: 0;
    border-bottom: 3px solid #666;
    padding-bottom: 0.2em;
  }
  h2 {
    font-size: 1.5em;
    margin-top: 0.5em;
    margin-bottom: 0.4em;
    color: #1e50a2;
  }
  h3 {
    font-size: 1.3em;
    margin-top: 0.5em;
    margin-bottom: 0.4em;
    color: #333;
    font-weight: bold;
  }
  ul, ol {
    margin-top: 0.5em;
    margin-bottom: 0.5em;
    padding-left: 1.5em;
  }
  li {
    margin-bottom: 0.5em;
    line-height: 1.5;
  }
  table {
    font-size: 1.1em;
    margin: 0.8em 0;
    width: 100%;
    border-collapse: collapse;
  }
  th, td {
    padding: 8px 12px;
    border: 1px solid #ccc;
  }
  th {
    background-color: #e6edf7;
  }
  p {
    margin: 0.5em 0;
    line-height: 1.5;
  }
  strong {
    color: #1e50a2;
    font-weight: bold;
  }
  /* 図表のはみ出し防止設定 */
  section {
    overflow: hidden;
  }
  svg {
    max-width: 100%;
    height: auto;
    display: block;
    margin: 0 auto;
  }
  .chart-container, .pie-container, .flowchart-container, .sequence-container {
    max-width: 100%;
    overflow: hidden;
    margin: 0 auto;
  }
  img, div[style*="width"] {
    max-width: 100% !important;
    height: auto;
    box-sizing: border-box;
  }
  /* 共通コンテナスタイル */
  .container {
    margin: 20px 0;
  }
  /* 注釈スタイル */
  .note {
    font-size: 0.9em;
    color: #666;
    font-style: italic;
    margin-top: 10px;
  }
  /* 強調ボックス */
  .highlight-box {
    background: #fff3cd;
    border: 1px solid #ffeaa7;
    border-radius: 5px;
    padding: 10px 15px;
    margin: 15px 0;
  }
  /* コードブロックスタイル */
  pre {
    background: #f4f4f4;
    border: 1px solid #ddd;
    border-radius: 5px;
    padding: 10px;
    overflow-x: auto;
    font-size: 0.9em;
  }
  code {
    background: #e9ecef;
    padding: 2px 6px;
    border-radius: 3px;
    font-size: 0.9em;
  }
---

<!-- 
このMARPテンプレートには以下の特徴があります：
1. 標準よりも大きいフォントサイズ（基本1.15em）
2. 見出しのスタイリング（H1には下線、H2はブルー色）
3. 表や箇条書きの最適化
4. 要素間の適切な余白設定
5. 視認性の高いカラースキーム

以下のスライドでは様々なデザインパターンが利用可能です：
- カード型レイアウト
- グリッドレイアウト
- 強調表示付きリスト
- スタイリングされた表
- SVG画像の埋め込み
- Mermaid図（フローチャート、シーケンス図など）
- Chart.jsグラフ（棒グラフ、円グラフなど）
-->

<!-- _class: title -->
<style scoped>
section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  padding: 0 60px;
}
h1 {
  font-size: 3em;
  margin-bottom: 1.2em;
  line-height: 1.4;
  border: none;
  color: #1e50a2;
}
.authors {
  font-size: 1.7em;
  line-height: 1.6;
  margin-top: 1em;
}
</style>

# プレゼンテーションタイトル

<div class="authors">

発表者名  
所属・肩書き

</div>

---

<!-- 
パターン1: シンプルなグリッドレイアウト
複数の項目を視覚的に分離する場合に使用
-->

# セクションタイトル1

## サブタイトル

<style scoped>
.grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 20px;
  margin-top: 25px;
  font-size: 1.2em;
}
.item {
  background: #f5f5f5;
  padding: 12px 20px;
  border-radius: 8px;
  border-left: 6px solid #1e50a2;
}
</style>

<div class="grid">

<div class="item">

### 項目1：
- **重要なポイント1**
- **重要なポイント2**
- **重要なポイント3**

</div>

<div class="item">

### 項目2：
- **重要なポイント1**
- **重要なポイント2**

</div>

</div>

---

<!-- 
パターン2: カード型リスト
各項目を個別のカードとして表示する場合に使用
-->

# セクションタイトル2

## サブタイトル

<style scoped>
.goals {
  font-size: 1.2em;
  margin-top: 25px;
}
.goal-item {
  background-color: #f0f5fa;
  margin-bottom: 20px;
  padding: 15px 20px;
  border-radius: 10px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}
.goal-title {
  font-weight: bold;
  color: #1e50a2;
  font-size: 1.1em;
  margin-bottom: 8px;
}
</style>

<div class="goals">

<div class="goal-item">
<div class="goal-title">1. 項目タイトル</div>
項目の詳細説明。簡潔かつ分かりやすい表現で記述します。
</div>

<div class="goal-item">
<div class="goal-title">2. 項目タイトル</div>
項目の詳細説明。簡潔かつ分かりやすい表現で記述します。
</div>

<div class="goal-item">
<div class="goal-title">3. 項目タイトル</div>
項目の詳細説明。簡潔かつ分かりやすい表現で記述します。
</div>

</div>

---

<!-- 
パターン3: アイコン型リスト
視覚的なブロックとして項目を表示する場合に使用
-->

# セクションタイトル3

## サブタイトル

<style scoped>
.methods {
  font-size: 1.2em;
  margin-top: 25px;
}
.method-item {
  background-color: #f8f9fa;
  margin-bottom: 15px;
  padding: 12px 20px;
  border-radius: 8px;
  border-left: 5px solid #4472C4;
}
.method-title {
  font-weight: bold;
  margin-bottom: 8px;
}
</style>

<div class="methods">

<div class="method-item">
<div class="method-title">小見出し1</div>
ここに詳細テキストを記述します。箇条書きや短い文章で説明します。
</div>

<div class="method-item">
<div class="method-title">小見出し2</div>
ここに詳細テキストを記述します。<br>
改行を使用して読みやすくすることも可能です。
</div>

<div class="method-item">
<div class="method-title">小見出し3</div>
ここに詳細テキストを記述します。表やリストの埋め込みも可能です。
</div>

</div>

---

<!-- 
パターン4: 表組み
データを整理して表示する場合に使用
-->

# セクションタイトル4

## サブタイトル

<style scoped>
table {
  width: 100%;
  font-size: 1.2em;
  margin-top: 20px;
}
th {
  background-color: #e6edf7;
  text-align: center;
  font-weight: bold;
}
th, td {
  padding: 10px 15px;
}
.highlight {
  font-weight: bold;
  color: #1e50a2;
}
</style>

| 項目1 | 項目2 | 項目3 | 項目4 |
| ----- | ----- | ----- | ----- |
| データ1 | データ2 | <span class="highlight">強調データ</span> | データ4 |
| データ5 | データ6 | <span class="highlight">強調データ</span> | データ8 |
| データ9 | データ10 | データ11 | データ12 |

---

<!-- 
パターン5: 画像挿入
SVGやPNG画像を中央に表示する場合に使用
-->

# セクションタイトル5

## サブタイトル

<style scoped>
.image-container {
  margin-top: 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.chart {
  width: 100%;
  max-width: 800px;
  height: auto;
  margin: 10px 0 20px 0;
}
.image-caption {
  font-style: italic;
  color: #666;
  text-align: center;
  margin-top: 10px;
}
</style>

<div class="image-container">

<!-- ここにSVGまたは画像ファイルを挿入 -->
<!-- ![](path/to/your/image.png) -->
<svg width="100%" height="300" viewBox="0 0 600 300" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet">
  <!-- サンプルグラフ -->
  <rect x="50" y="50" width="80" height="200" fill="#4472C4" />
  <rect x="180" y="100" width="80" height="150" fill="#ED7D31" />
  <rect x="310" y="80" width="80" height="170" fill="#A5A5A5" />
  <rect x="440" y="120" width="80" height="130" fill="#FFC000" />
  
  <!-- 軸 -->
  <line x1="50" y1="250" x2="520" y2="250" stroke="black" stroke-width="2"/>
  <line x1="50" y1="50" x2="50" y2="250" stroke="black" stroke-width="2"/>
  
  <!-- ラベル -->
  <text x="90" y="270" text-anchor="middle" font-size="14">項目1</text>
  <text x="220" y="270" text-anchor="middle" font-size="14">項目2</text>
  <text x="350" y="270" text-anchor="middle" font-size="14">項目3</text>
  <text x="480" y="270" text-anchor="middle" font-size="14">項目4</text>
</svg>

<div class="image-caption">
図1: SVGで作成したサンプルグラフ
</div>

</div>

---

<!-- 
パターン6: 問題と解決策
対比して表示したい場合に使用
-->

# セクションタイトル6

## サブタイトル

<style scoped>
.problems {
  margin-top: 15px;
  font-size: 1.2em;
  width: 100%;
}
.problem-item {
  background: #f5f5f5;
  padding: 10px 15px;
  margin-bottom: 10px;
  border-radius: 6px;
  display: flex;
  align-items: center;
}
.problem-problem {
  font-weight: bold;
  margin-right: 10px;
}
.problem-arrow {
  margin: 0 10px;
  color: #666;
}
.problem-solution {
  color: #1e50a2;
}
</style>

<div class="problems">
<div class="problem-item">
<span class="problem-problem">問題点1</span>
<span class="problem-arrow">→</span>
<span class="problem-solution">解決策または対応方法の説明</span>
</div>

<div class="problem-item">
<span class="problem-problem">問題点2</span>
<span class="problem-arrow">→</span>
<span class="problem-solution">解決策または対応方法の説明</span>
</div>

<div class="problem-item">
<span class="problem-problem">問題点3</span>
<span class="problem-arrow">→</span>
<span class="problem-solution">解決策または対応方法の説明</span>
</div>
</div>

---

<!-- 
パターン7: 予算表
数値データに強調を入れる場合に使用
-->

# セクションタイトル7

## サブタイトル

<style scoped>
.budget-container {
  margin-top: 20px;
  font-size: 1.2em;
}
.budget-title {
  font-size: 1.2em;
  margin-bottom: 15px;
  font-weight: bold;
  color: #1e50a2;
  background-color: #e6edf7;
  padding: 10px;
  border-radius: 5px;
  text-align: center;
}
table {
  width: 100%;
  font-size: 1.2em;
}
th {
  background-color: #e6edf7;
  text-align: center;
}
th, td {
  padding: 12px 15px;
}
.amount {
  font-weight: bold;
  color: #d04255;
}
</style>

<div class="budget-container">

<div class="budget-title">予算表</div>

| 項目 | 金額 | 詳細 |
| ----- | ----- | ----- |
| 項目1 | <span class="amount">xxx円</span> | 項目の詳細説明 |
| 項目2 | <span class="amount">xxx円</span> | 項目の詳細説明 |
| 項目3 | <span class="amount">xxx円</span> | 項目の詳細説明 |

</div>

---

<!-- 
パターン8: 箇条書きリスト
重要な項目を強調表示する場合に使用
-->

# セクションタイトル8

## サブタイトル

<style scoped>
.human-resource {
  margin-top: 25px;
  font-size: 1.2em;
}
.contribution-box {
  background: #f5f5f5;
  padding: 20px;
  border-radius: 10px;
  margin-bottom: 25px;
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}
.contribution-title {
  font-weight: bold;
  color: #1e50a2;
  font-size: 1.2em;
  margin-bottom: 15px;
  border-bottom: 2px solid #1e50a2;
  padding-bottom: 5px;
}
.contribution-item {
  margin-bottom: 12px;
  padding-left: 25px;
  position: relative;
}
.contribution-item:before {
  content: "●";
  color: #1e50a2;
  position: absolute;
  left: 0;
  font-size: 0.8em;
  top: 0.2em;
}
</style>

<div class="human-resource">

<div class="contribution-box">
<div class="contribution-title">大見出し1</div>

<div class="contribution-item">
リスト項目1
</div>

<div class="contribution-item">
リスト項目2
</div>

<div class="contribution-item">
リスト項目3
</div>
</div>

<div class="contribution-box">
<div class="contribution-title">大見出し2</div>

<div class="contribution-item">
リスト項目1
</div>

<div class="contribution-item">
リスト項目2
</div>
</div>

</div>

---

<!-- 
パターン9: 2列グリッド
情報を横に2列で表示する場合に使用
-->

# セクションタイトル9

<style scoped>
.special-notes {
  margin-top: 40px;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 25px;
  font-size: 1.25em;
}
.note-item {
  background: #f5f5f5;
  padding: 20px;
  border-radius: 10px;
  line-height: 1.6;
  box-shadow: 0 3px 6px rgba(0,0,0,0.1);
  border-top: 5px solid #1e50a2;
  height: 100%;
  display: flex;
  align-items: center;
}
</style>

<div class="special-notes">

<div class="note-item">
項目1の説明文。簡潔かつ分かりやすい表現で記述します。
</div>

<div class="note-item">
項目2の説明文。簡潔かつ分かりやすい表現で記述します。
</div>

<div class="note-item">
項目3の説明文。簡潔かつ分かりやすい表現で記述します。
</div>

<div class="note-item">
項目4の説明文。簡潔かつ分かりやすい表現で記述します。
</div>

</div>

---

<!-- 
パターン10: SVGフローチャート
プロセスフローをSVGで表示
重要: viewBoxの高さはすべての要素が収まるように設定すること
-->

# SVGフローチャートの例

## プロセスフローの可視化

<style scoped>
.flowchart-container {
  margin: 20px auto;
  max-width: 75%;
  display: flex;
  justify-content: center;
  overflow: hidden;
}
</style>

<div class="flowchart-container">

<svg width="100%" height="350" viewBox="0 0 600 450" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet">
  <!-- 開始 -->
  <rect x="250" y="20" width="100" height="40" rx="20" fill="#f9f" stroke="#333" stroke-width="2"/>
  <text x="300" y="45" text-anchor="middle" font-size="14">開始</text>
  
  <!-- 条件判定 -->
  <polygon points="300,90 350,125 300,160 250,125" fill="#bbf" stroke="#333" stroke-width="2"/>
  <text x="300" y="130" text-anchor="middle" font-size="13">条件判定</text>
  
  <!-- 処理1 -->
  <rect x="100" y="190" width="100" height="40" fill="#e6edf7" stroke="#333" stroke-width="2"/>
  <text x="150" y="215" text-anchor="middle" font-size="13">処理1</text>
  
  <!-- 処理2 -->
  <rect x="400" y="190" width="100" height="40" fill="#e6edf7" stroke="#333" stroke-width="2"/>
  <text x="450" y="215" text-anchor="middle" font-size="13">処理2</text>
  
  <!-- 結果出力 -->
  <rect x="250" y="260" width="100" height="40" fill="#e6edf7" stroke="#333" stroke-width="2"/>
  <text x="300" y="285" text-anchor="middle" font-size="13">結果出力</text>
  
  <!-- 終了 -->
  <rect x="250" y="330" width="100" height="40" rx="20" fill="#f9f" stroke="#333" stroke-width="2"/>
  <text x="300" y="355" text-anchor="middle" font-size="14">終了</text>
  
  <!-- 矢印 -->
  <defs>
    <marker id="arrowhead" markerWidth="10" markerHeight="7" refX="10" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#333" />
    </marker>
  </defs>
  
  <line x1="300" y1="60" x2="300" y2="90" stroke="#333" stroke-width="2" marker-end="url(#arrowhead)"/>
  <line x1="250" y1="125" x2="200" y2="190" stroke="#333" stroke-width="2" marker-end="url(#arrowhead)"/>
  <line x1="350" y1="125" x2="400" y2="190" stroke="#333" stroke-width="2" marker-end="url(#arrowhead)"/>
  <line x1="150" y1="230" x2="250" y2="270" stroke="#333" stroke-width="2" marker-end="url(#arrowhead)"/>
  <line x1="450" y1="230" x2="350" y2="270" stroke="#333" stroke-width="2" marker-end="url(#arrowhead)"/>
  <line x1="300" y1="300" x2="300" y2="330" stroke="#333" stroke-width="2" marker-end="url(#arrowhead)"/>
  
  <!-- ラベル -->
  <text x="210" y="115" text-anchor="middle" font-size="12">はい</text>
  <text x="390" y="115" text-anchor="middle" font-size="12">いいえ</text>
</svg>

</div>

**ポイント：** SVGを使用することで、PDFエクスポート時も確実に表示されます。

---

<!-- 
パターン11: SVGシーケンス図
システム間の相互作用をSVGで表示
重要: viewBoxの高さはすべての要素が収まるように設定すること
-->

# SVGシーケンス図の例

## システム間の相互作用

<style scoped>
.sequence-container {
  margin: 10px auto;
  max-width: 70%;
  display: flex;
  justify-content: center;
  overflow: hidden;
}
</style>

<div class="sequence-container">

<svg width="100%" height="320" viewBox="0 0 650 310" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet">
  <!-- 参加者 -->
  <rect x="50" y="20" width="100" height="40" fill="#e6edf7" stroke="#333" stroke-width="2"/>
  <text x="100" y="45" text-anchor="middle" font-size="14">ユーザー</text>
  
  <rect x="275" y="20" width="100" height="40" fill="#e6edf7" stroke="#333" stroke-width="2"/>
  <text x="325" y="45" text-anchor="middle" font-size="14">システム</text>
  
  <rect x="500" y="20" width="100" height="40" fill="#e6edf7" stroke="#333" stroke-width="2"/>
  <text x="550" y="45" text-anchor="middle" font-size="14">データベース</text>
  
  <!-- ライフライン -->
  <line x1="100" y1="60" x2="100" y2="270" stroke="#333" stroke-width="2" stroke-dasharray="5,5"/>
  <line x1="325" y1="60" x2="325" y2="270" stroke="#333" stroke-width="2" stroke-dasharray="5,5"/>
  <line x1="550" y1="60" x2="550" y2="270" stroke="#333" stroke-width="2" stroke-dasharray="5,5"/>
  
  <!-- メッセージ -->
  <defs>
    <marker id="arrow" markerWidth="10" markerHeight="7" refX="10" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#333" />
    </marker>
  </defs>
  
  <!-- リクエスト送信 -->
  <line x1="100" y1="100" x2="320" y2="100" stroke="#333" stroke-width="2" marker-end="url(#arrow)"/>
  <text x="210" y="95" text-anchor="middle" font-size="12">リクエスト送信</text>
  
  <!-- データ照会 -->
  <line x1="325" y1="140" x2="545" y2="140" stroke="#333" stroke-width="2" marker-end="url(#arrow)"/>
  <text x="435" y="135" text-anchor="middle" font-size="12">データ照会</text>
  
  <!-- データ返却 -->
  <line x1="550" y1="180" x2="330" y2="180" stroke="#333" stroke-width="2" stroke-dasharray="5,3" marker-end="url(#arrow)"/>
  <text x="440" y="175" text-anchor="middle" font-size="12">データ返却</text>
  
  <!-- レスポンス返却 -->
  <line x1="325" y1="220" x2="105" y2="220" stroke="#333" stroke-width="2" stroke-dasharray="5,3" marker-end="url(#arrow)"/>
  <text x="215" y="215" text-anchor="middle" font-size="12">レスポンス返却</text>
  
  <!-- ノート -->
  <rect x="50" y="240" width="275" height="25" fill="#fff3cd" stroke="#ffc107" stroke-width="1" rx="5"/>
  <text x="187" y="257" text-anchor="middle" font-size="11">処理完了</text>
</svg>

</div>

**ポイント：** SVGを使用することで、シーケンス図も確実に表示されます。

---

<!-- 
パターン12: SVG円グラフ
データの割合をSVGで表示
-->

# SVG円グラフの例

## プロジェクト工数配分

<style scoped>
.pie-container {
  margin: 20px auto;
  max-width: 60%;
  display: flex;
  justify-content: center;
  overflow: hidden;
}
.chart-description {
  text-align: center;
  margin-top: 20px;
  font-size: 1.1em;
  color: #666;
}
</style>

<div class="pie-container">

<!-- テーブルベースの円グラフ風表示 -->
<div style="display: flex; justify-content: center; align-items: center; gap: 40px;">
  <div style="width: 250px; height: 250px; border-radius: 50%; background: conic-gradient(#4472C4 0deg 108deg, #ED7D31 108deg 270deg, #A5A5A5 270deg 342deg, #FFC000 342deg 360deg); box-shadow: 0 4px 8px rgba(0,0,0,0.2);"></div>
  <div style="font-size: 1.1em;">
    <div style="margin-bottom: 15px;"><span style="display: inline-block; width: 20px; height: 20px; background: #4472C4; margin-right: 10px;"></span>設計: 30%</div>
    <div style="margin-bottom: 15px;"><span style="display: inline-block; width: 20px; height: 20px; background: #ED7D31; margin-right: 10px;"></span>実装: 45%</div>
    <div style="margin-bottom: 15px;"><span style="display: inline-block; width: 20px; height: 20px; background: #A5A5A5; margin-right: 10px;"></span>テスト: 20%</div>
    <div style="margin-bottom: 15px;"><span style="display: inline-block; width: 20px; height: 20px; background: #FFC000; margin-right: 10px;"></span>その他: 5%</div>
  </div>
</div>

</div>

<div class="chart-description">
総工数：100人日
</div>

**ポイント：** SVGを使用することで、円グラフも確実に表示されます。

---

<!-- 
パターン13: Chart.jsを使った棒グラフ
MARPでChart.jsを使用する場合のテンプレート
-->

# Chart.jsグラフの例：棒グラフ

## 月別売上データ

<style scoped>
.chart-container {
  margin: 20px auto;
  width: 80%;
  max-width: 100%;
  overflow: hidden;
  box-sizing: border-box;
}
.chart-note {
  text-align: center;
  margin-top: 15px;
  padding: 10px;
  background: #f8f9fa;
  border-radius: 5px;
  font-size: 0.9em;
}
</style>

<div class="chart-container">

<!-- シンプルなSVG棒グラフ -->
<svg width="100%" height="350" viewBox="0 0 700 400" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet">
  <!-- グラフエリア -->
  <rect x="50" y="50" width="600" height="280" fill="#f8f9fa" stroke="#ddd"/>
  
  <!-- 棒グラフ -->
  <rect x="80" y="210" width="80" height="120" fill="#4472C4"/>
  <rect x="180" y="150" width="80" height="180" fill="#4472C4"/>
  <rect x="280" y="198" width="80" height="132" fill="#4472C4"/>
  <rect x="380" y="180" width="80" height="150" fill="#4472C4"/>
  <rect x="480" y="102" width="80" height="228" fill="#4472C4"/>
  <rect x="580" y="138" width="80" height="192" fill="#4472C4"/>
  
  <!-- X軸 -->
  <line x1="50" y1="330" x2="650" y2="330" stroke="black" stroke-width="2"/>
  <!-- Y軸 -->
  <line x1="50" y1="50" x2="50" y2="330" stroke="black" stroke-width="2"/>
  
  <!-- X軸ラベル -->
  <text x="120" y="350" text-anchor="middle" font-size="14">1月</text>
  <text x="220" y="350" text-anchor="middle" font-size="14">2月</text>
  <text x="320" y="350" text-anchor="middle" font-size="14">3月</text>
  <text x="420" y="350" text-anchor="middle" font-size="14">4月</text>
  <text x="520" y="350" text-anchor="middle" font-size="14">5月</text>
  <text x="620" y="350" text-anchor="middle" font-size="14">6月</text>
  
  <!-- Y軸ラベル -->
  <text x="40" y="55" text-anchor="end" font-size="12">25</text>
  <text x="40" y="110" text-anchor="end" font-size="12">20</text>
  <text x="40" y="165" text-anchor="end" font-size="12">15</text>
  <text x="40" y="220" text-anchor="end" font-size="12">10</text>
  <text x="40" y="275" text-anchor="end" font-size="12">5</text>
  <text x="40" y="330" text-anchor="end" font-size="12">0</text>
  
  <!-- タイトル -->
  <text x="350" y="30" text-anchor="middle" font-size="16" font-weight="bold">売上高（百万円）</text>
</svg>

</div>

<div class="chart-note">
※ SVGを使用しているため、PDFエクスポート時も正しく表示されます
</div>

---

<!-- 
パターン14: 複合レイアウト（テキスト + SVG図）
テキスト説明とSVG図を組み合わせる場合
-->

# 複合レイアウトの例

## プロセス説明と図解

<style scoped>
.content-grid {
  display: grid;
  grid-template-columns: 1fr 1.2fr;
  gap: 30px;
  align-items: start;
  margin-top: 20px;
}
.text-content {
  font-size: 1.1em;
  line-height: 1.6;
}
.text-content h3 {
  margin-top: 0;
  margin-bottom: 10px;
}
.mermaid-container {
  background: #f8f9fa;
  padding: 15px;
  border-radius: 8px;
  display: flex;
  justify-content: center;
}
.mermaid {
  font-size: 0.8em !important;
}
</style>

<div class="content-grid">

<div class="text-content">

### プロセスの概要

1. **要件定義**  
   顧客のニーズを明確化

2. **設計フェーズ**  
   システム構成を決定

3. **実装・テスト**  
   品質を確保しながら開発

4. **リリース**  
   本番環境への展開

</div>

<div class="mermaid-container">

```mermaid
flowchart TD
    A[要件定義] --> B[設計]
    B --> C[実装]
    C --> D[テスト]
    D --> E{品質OK?}
    E -->|はい| F[リリース]
    E -->|いいえ| C
    
    style A fill:#e6edf7
    style F fill:#d4edda
```

</div>

</div>

---

<!-- 
パターン15: サイズ制限のベストプラクティス
Mermaid図とChart.jsのサイズ調整ガイド
-->

# 図表サイズ制限のベストプラクティス

## MARPでの効果的な図表表示

<style scoped>
.best-practices {
  margin-top: 20px;
  font-size: 1.15em;
}
.practice-item {
  background: #f0f5fa;
  margin: 15px 0;
  padding: 15px 20px;
  border-radius: 8px;
  border-left: 5px solid #1e50a2;
}
.practice-title {
  font-weight: bold;
  color: #1e50a2;
  margin-bottom: 8px;
}
code {
  background: #e9ecef;
  padding: 2px 6px;
  border-radius: 3px;
  font-size: 0.9em;
}
</style>

<div class="best-practices">

<div class="practice-item">
<div class="practice-title">1. Mermaid図のサイズ調整</div>
• コンテナに <code>max-width: 80-90%</code> を設定<br>
• フォントサイズを <code>0.8-0.9em</code> に調整<br>
• 複雑な図は分割して複数スライドに配置
</div>

<div class="practice-item">
<div class="practice-title">2. Chart.jsグラフの制約</div>
• <code>responsive: true</code> と <code>maintainAspectRatio: false</code> を設定<br>
• コンテナの高さを固定値（400-500px）に設定<br>
• PDFエクスポート時は静的画像を使用
</div>

<div class="practice-item">
<div class="practice-title">3. 複合レイアウトの工夫</div>
• グリッドレイアウトで図とテキストを配置<br>
• 図の背景色で視覚的な分離を実現<br>
• 余白を適切に設定して読みやすさを確保
</div>

</div>

---

<!-- 
パターン16: タイムライン表示
時系列の情報を視覚的に表示する場合に使用
-->

# タイムライン表示の例

## プロジェクトの進行スケジュール

<style scoped>
.timeline {
  margin: 30px 0;
  position: relative;
  padding-left: 40px;
}
.timeline::before {
  content: '';
  position: absolute;
  left: 15px;
  top: 0;
  bottom: 0;
  width: 3px;
  background: #1e50a2;
}
.timeline-item {
  position: relative;
  margin-bottom: 25px;
  padding-left: 30px;
}
.timeline-item::before {
  content: '';
  position: absolute;
  left: -25px;
  top: 5px;
  width: 15px;
  height: 15px;
  border-radius: 50%;
  background: #1e50a2;
  border: 3px solid #fff;
  box-shadow: 0 0 0 3px #1e50a2;
}
.timeline-date {
  font-weight: bold;
  color: #1e50a2;
  margin-bottom: 5px;
}
.timeline-content {
  background: #f8f9fa;
  padding: 10px 15px;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}
</style>

<div class="timeline">

<div class="timeline-item">
<div class="timeline-date">2024年1月</div>
<div class="timeline-content">
要件定義フェーズ - 顧客ヒアリングと要求分析
</div>
</div>

<div class="timeline-item">
<div class="timeline-date">2024年2月</div>
<div class="timeline-content">
基本設計 - システムアーキテクチャの決定
</div>
</div>

<div class="timeline-item">
<div class="timeline-date">2024年3月</div>
<div class="timeline-content">
詳細設計・実装開始 - 主要機能の開発
</div>
</div>

<div class="timeline-item">
<div class="timeline-date">2024年4月</div>
<div class="timeline-content">
テスト・リリース準備 - 品質保証と展開準備
</div>
</div>

</div>

---

<!-- 
パターン17: 比較表（色分け付き）
複数の選択肢を視覚的に比較する場合に使用
-->

# 比較表の例

## 技術スタックの選定

<style scoped>
.comparison-table {
  width: 100%;
  margin-top: 20px;
  border-collapse: collapse;
  font-size: 1.1em;
}
.comparison-table th {
  background: #1e50a2;
  color: white;
  padding: 12px;
  text-align: center;
  font-weight: bold;
}
.comparison-table td {
  padding: 10px;
  border: 1px solid #ddd;
  text-align: center;
}
.comparison-table tr:nth-child(even) {
  background: #f8f9fa;
}
.excellent {
  background: #d4edda !important;
  color: #155724;
  font-weight: bold;
}
.good {
  background: #cce5ff !important;
  color: #004085;
}
.fair {
  background: #fff3cd !important;
  color: #856404;
}
</style>

<table class="comparison-table">
<thead>
<tr>
<th>評価項目</th>
<th>技術A</th>
<th>技術B</th>
<th>技術C</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>パフォーマンス</strong></td>
<td class="excellent">◎</td>
<td class="good">○</td>
<td class="fair">△</td>
</tr>
<tr>
<td><strong>学習コスト</strong></td>
<td class="fair">△</td>
<td class="excellent">◎</td>
<td class="good">○</td>
</tr>
<tr>
<td><strong>コミュニティ</strong></td>
<td class="good">○</td>
<td class="excellent">◎</td>
<td class="good">○</td>
</tr>
<tr>
<td><strong>保守性</strong></td>
<td class="excellent">◎</td>
<td class="good">○</td>
<td class="excellent">◎</td>
</tr>
</tbody>
</table>

<div class="note">
◎：優秀　○：良好　△：普通
</div>

---

<!-- 
パターン18: アイコン付きリスト（Font Awesome風）
視覚的にわかりやすいリストを作成する場合に使用
-->

# アイコン付きリストの例

## システムの主要機能

<style scoped>
.icon-list {
  margin-top: 30px;
  font-size: 1.2em;
}
.icon-item {
  display: flex;
  align-items: flex-start;
  margin-bottom: 20px;
  padding: 15px;
  background: #f8f9fa;
  border-radius: 8px;
  transition: all 0.3s ease;
}
.icon-item:hover {
  background: #e9ecef;
  transform: translateX(5px);
}
.icon {
  flex-shrink: 0;
  width: 40px;
  height: 40px;
  margin-right: 15px;
  background: #1e50a2;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: 20px;
  font-weight: bold;
}
.icon-content h4 {
  margin: 0 0 5px 0;
  color: #1e50a2;
}
.icon-content p {
  margin: 0;
  line-height: 1.5;
}
</style>

<div class="icon-list">

<div class="icon-item">
<div class="icon">📊</div>
<div class="icon-content">
<h4>データ分析機能</h4>
<p>リアルタイムでデータを収集・分析し、ビジュアライゼーションを提供</p>
</div>
</div>

<div class="icon-item">
<div class="icon">🔒</div>
<div class="icon-content">
<h4>セキュリティ管理</h4>
<p>高度な暗号化と認証システムによる堅牢なセキュリティ</p>
</div>
</div>

<div class="icon-item">
<div class="icon">🚀</div>
<div class="icon-content">
<h4>パフォーマンス最適化</h4>
<p>自動スケーリングとキャッシュ機構による高速処理</p>
</div>
</div>

<div class="icon-item">
<div class="icon">🔄</div>
<div class="icon-content">
<h4>自動同期機能</h4>
<p>複数デバイス間でのデータ自動同期とバックアップ</p>
</div>
</div>

</div>

---

<!-- 
パターン19: 進捗インジケーター
進捗状況を視覚的に表示する場合に使用
-->

# 進捗インジケーターの例

## プロジェクト進捗状況

<style scoped>
.progress-container {
  margin: 30px 0;
  font-size: 1.15em;
}
.progress-item {
  margin-bottom: 25px;
}
.progress-label {
  display: flex;
  justify-content: space-between;
  margin-bottom: 8px;
  font-weight: bold;
}
.progress-bar {
  width: 100%;
  height: 25px;
  background: #e9ecef;
  border-radius: 12px;
  overflow: hidden;
  position: relative;
}
.progress-fill {
  height: 100%;
  background: linear-gradient(90deg, #1e50a2 0%, #4472C4 100%);
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  padding-right: 10px;
  color: white;
  font-weight: bold;
  font-size: 0.9em;
  transition: width 0.3s ease;
}
.milestone {
  margin-top: 20px;
  padding: 15px;
  background: #d4edda;
  border-radius: 8px;
  border-left: 5px solid #28a745;
}
</style>

<div class="progress-container">

<div class="progress-item">
<div class="progress-label">
<span>要件定義</span>
<span>100%</span>
</div>
<div class="progress-bar">
<div class="progress-fill" style="width: 100%">完了</div>
</div>
</div>

<div class="progress-item">
<div class="progress-label">
<span>設計フェーズ</span>
<span>80%</span>
</div>
<div class="progress-bar">
<div class="progress-fill" style="width: 80%">80%</div>
</div>
</div>

<div class="progress-item">
<div class="progress-label">
<span>実装</span>
<span>45%</span>
</div>
<div class="progress-bar">
<div class="progress-fill" style="width: 45%">45%</div>
</div>
</div>

<div class="progress-item">
<div class="progress-label">
<span>テスト</span>
<span>10%</span>
</div>
<div class="progress-bar">
<div class="progress-fill" style="width: 10%">10%</div>
</div>
</div>

<div class="milestone">
<strong>次のマイルストーン：</strong> 設計フェーズ完了（予定：2024年3月15日）
</div>

</div>

---

<!-- 
パターン20: まとめスライド
要点をまとめて表示する場合に使用
-->

# まとめ

## 本日のプレゼンテーションの要点

<style scoped>
.summary-container {
  margin-top: 30px;
}
.summary-box {
  background: linear-gradient(135deg, #f5f7fa 0%, #e9ecef 100%);
  border-radius: 15px;
  padding: 30px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  margin-bottom: 20px;
}
.summary-title {
  font-size: 1.4em;
  color: #1e50a2;
  margin-bottom: 20px;
  text-align: center;
  font-weight: bold;
}
.key-points {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
  margin-bottom: 25px;
}
.key-point {
  background: white;
  padding: 20px;
  border-radius: 10px;
  border-left: 4px solid #1e50a2;
  box-shadow: 0 2px 5px rgba(0,0,0,0.05);
}
.key-point h4 {
  color: #1e50a2;
  margin: 0 0 10px 0;
}
.key-point p {
  margin: 0;
  line-height: 1.5;
}
.action-items {
  background: #fff3cd;
  border: 1px solid #ffeaa7;
  border-radius: 10px;
  padding: 20px;
  margin-top: 20px;
}
.action-items h4 {
  color: #856404;
  margin: 0 0 10px 0;
}
.action-items ul {
  margin: 0;
  padding-left: 20px;
}
</style>

<div class="summary-container">

<div class="summary-box">
<div class="summary-title">🎯 重要ポイント</div>

<div class="key-points">
<div class="key-point">
<h4>1. 現状の課題</h4>
<p>システムの老朽化とパフォーマンスの低下が主要な問題</p>
</div>

<div class="key-point">
<h4>2. 提案ソリューション</h4>
<p>クラウドネイティブな新システムへの段階的移行</p>
</div>

<div class="key-point">
<h4>3. 期待効果</h4>
<p>処理速度50%向上、運用コスト30%削減</p>
</div>

<div class="key-point">
<h4>4. 実施期間</h4>
<p>2024年1月〜6月（6ヶ月間）</p>
</div>
</div>

<div class="action-items">
<h4>📋 次のアクション</h4>
<ul>
<li>詳細な要件定義書の作成（〜2月末）</li>
<li>ベンダー選定とRFP作成（3月中旬）</li>
<li>予算承認プロセスの開始（3月末）</li>
</ul>
</div>

</div>

</div> 