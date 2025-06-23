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
![](path/to/your/image.png)

<div class="image-caption">
図1: 画像の説明文をここに記載
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