<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8" />
  <title>トップページワイヤーフレーム - 「コンプリエイト（仮）」例</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <!-- 簡易なCSSを内包：ブラウザでプレビューすればそれなりの見た目で表示されます -->
  <style>
    * {
      box-sizing: border-box;
      margin: 0; 
      padding: 0;
      font-family: sans-serif;
      color: #333;
    }
    body {
      background: #f9f9f9;
      line-height: 1.5;
    }
    header, nav, footer, section {
      width: 100%;
      margin: 0 auto;
      max-width: 1200px;
      padding: 20px;
    }
    header, footer {
      background: #f0f0f0;
    }
    h1, h2, h3 {
      margin-bottom: 10px;
      font-weight: normal;
    }
    a, button {
      cursor: pointer;
      text-decoration: none;
    }
    a, button:hover {
      opacity: 0.9;
    }
    /* Heroセクション */
    .hero {
      background: #e6f1ff; /* ヒーローバック色 */
      text-align: center;
      padding: 60px 20px;
      margin-bottom: 20px;
      border-radius: 6px;
    }
    .hero h1 {
      font-size: 2rem;
      margin-bottom: 16px;
      font-weight: bold;
    }
    .hero p {
      font-size: 1.1rem;
      margin-bottom: 24px;
      color: #444;
    }
    .cta-buttons {
      display: inline-flex;
      gap: 10px;
      flex-wrap: wrap;
      justify-content: center;
    }
    .cta-buttons a, .cta-buttons button {
      background: #0078ff;
      color: #fff;
      padding: 12px 20px;
      border-radius: 4px;
      font-size: 1rem;
      border: none;
      transition: background 0.2s ease;
    }
    .cta-buttons a:active, .cta-buttons button:active {
      background: #005dc1; 
    }
    /* 各セクション */
    section {
      background: #fff;
      margin-bottom: 20px;
      border-radius: 6px;
      box-shadow: 0 0 4px rgba(0,0,0,0.05);
    }
    section h2 {
      margin-bottom: 10px;
      font-size: 1.4rem;
    }
    section > div {
      padding: 20px;
    }
    /* 特徴やステップのスタイル */
    .features-list > div, 
    .steps-list > div {
      margin-bottom: 16px;
    }
    .features-list h3, .steps-list h4 {
      margin-bottom: 6px;
      font-weight: bold;
      font-size: 1.1rem;
      color: #0078ff;
    }
    /* 料金セクション: テーブル */
    .compare-table {
      margin-top: 20px;
      border-collapse: collapse;
      width: 100%;
      background: #fafafa;
    }
    .compare-table th,
    .compare-table td {
      border: 1px solid #ccc;
      padding: 12px;
      text-align: left;
    }
    .highlight {
      color: #0078ff;
      font-weight: bold;
    }
    /* FAQ */
    .faq-list > div {
      margin-bottom: 16px;
    }
    .faq-list strong {
      color: #0078ff;
    }
    /* お問い合わせボタンなど */
    .contact-section button {
      background: #0078ff;
      color: #fff;
      border: none;
      padding: 10px 18px;
      border-radius: 4px;
      font-size: 1rem;
      margin-right: 10px;
      margin-top: 10px;
    }
    .contact-section button:active {
      background: #005dc1;
    }
    .mw-700 {
      max-width: 700px;
      margin: 0 auto;
    }
    /* フッター */
    footer {
      text-align: center;
      background: #f0f0f0;
      margin-top: 20px;
      padding: 30px;
      font-size: 0.9rem;
    }
    footer p {
      margin: 5px 0;
    }
  </style>
</head>
<body>

<header>
  <nav>
    <h2>コンプリエイトホームページ（仮）</h2>
  </nav>
</header>

<!-- HERO SECTION -->
<section class="hero">
  <h1>写真や文章の準備を大幅に減らせる<br>あなただけのホームページをスムーズに</h1>
  <p>
    多彩な業種に合う写真や例文を取りそろえています。<br>
    難しい操作なしで形にできるから、本業に専念できる。
  </p>
  <div class="cta-buttons">
    <a href="#">無料で相談してみる</a>
    <a href="#">30日間お試しはこちら</a>
  </div>
</section>

<!-- FEATURES SECTION -->
<section class="features">
  <div>
    <h2>なぜ「手間を大きく減らせる」の？</h2>
    <div class="features-list">
      <div>
        <h3>1. 豊富な写真＆文章サンプル</h3>
        <p>
          業種別のイメージ画像や文章例を豊富に用意。<br>
          すべてをご自分で作成しなくても、ベースとなる素材を使って素早く整えられます。
        </p>
      </div>
      <div>
        <h3>2. 更新しやすい管理画面</h3>
        <p>
          専門知識がなくても操作しやすいUIを採用。<br>
          定期的な写真差し替えや文章の追加修正も、短時間で済ませられます。
        </p>
      </div>
      <div>
        <h3>3. 特許取得のシステムで検索リスク軽減</h3>
        <p>
          共有コンテンツを活用しても重複ペナルティを最小限に。<br>
          月額の中にこの仕組みの維持費が含まれています。
        </p>
      </div>
    </div>
  </div>
</section>

<!-- STEPS SECTION -->
<section class="steps">
  <div>
    <h2>サイト公開までの流れ</h2>
    <div class="steps-list">
      <div>
        <h4>ステップ1：基本情報を登録</h4>
        <p>事業内容や業種などを簡単に入力するだけ。</p>
      </div>
      <div>
        <h4>ステップ2：写真・例文を選ぶ</h4>
        <p>当社が保有するサンプルから合いそうなものを選択。<br>オリジナル写真の追加も可能です。</p>
      </div>
      <div>
        <h4>ステップ3：独自情報を補足</h4>
        <p>店舗名や料金情報など最低限の部分だけ追記すれば、全体が整います。</p>
      </div>
      <div>
        <h4>ステップ4：公開ボタンで完成</h4>
        <p>調整次第で数日ほどで形に。ゆっくりカスタマイズしながら仕上げることもできます。</p>
      </div>
    </div>
  </div>
</section>

<!-- PRICING SECTION -->
<section class="pricing">
  <div>
    <h2>料金プラン</h2>
    <div class="pricing-details">
      <div>
        <strong>初期費用：59,800円</strong><br>
        <span>業種別の写真・文章サンプル利用開始の費用。<br>
        撮影やライター外注をフルで行うより手間とコストを抑えられます。</span>
      </div>
      <br>
      <div>
        <strong>月額費用：5,980円</strong><br>
        <span>共有コンテンツ運用や特許取得の仕組み維持、<br>
        基本サポートが含まれます。</span>
      </div>
      
      <table class="compare-table">
        <thead>
          <tr>
            <th></th>
            <th>DIYノーコード</th>
            <th>フルオーダー</th>
            <th><span class="highlight">コンプリエイト</span></th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <th>初期コスト</th>
            <td>低〜無料<br>(撮影・執筆は自己負担)</td>
            <td>数十万円〜<br>(撮影・ライティング別)</td>
            <td>59,800円<br>(サンプル写真＆文章利用)</td>
          </tr>
          <tr>
            <th>更新コスト</th>
            <td>自力作業<br>時間と手間を要する</td>
            <td>更新のたび<br>制作会社に依頼費用</td>
            <td>月5,980円<br>(特許システム＆サポート含む)</td>
          </tr>
          <tr>
            <th>撮影・文章作成</th>
            <td>すべて自作</td>
            <td>プロ外注でコスト増</td>
            <td>大半をサンプルで補完しつつ<br>独自要素も追加OK</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</section>

<!-- INDUSTRIES / EXAMPLES -->
<section class="features">
  <div>
    <h2>こんな業種・目的の方におすすめ</h2>
    <div class="features-list">
      <div>
        <h3>美容サロン</h3>
        <p>季節スタイルやキャンペーンを手軽に写真追加し、PRできます。</p>
      </div>
      <div>
        <h3>建築・リフォーム</h3>
        <p>施工写真をベース素材に組み合わせ、ビフォアーアフター掲載もしやすく。</p>
      </div>
      <div>
        <h3>不動産</h3>
        <p>雛形写真で物件を魅力的に紹介。将来的に物件登録システムも検討中です。</p>
      </div>
      <!-- 他業種例も追加可能 -->
    </div>
    <p style="margin-top:20px;">
      上記以外にも、多数の業種に対応。<br>
      店舗やサービスのイメージ作りに時間をかけられない方に、特に向いています。
    </p>
  </div>
</section>

<!-- FAQ & SUPPORT -->
<section class="faq">
  <div>
    <h2>よくあるご質問</h2>
    <div class="faq-list">
      <div>
        <strong>Q:</strong>「写真や文章がすべて揃っている」とは？<br>
        <strong>A:</strong>多くの業種向け素材を取り揃えていますが、店舗情報など最低限の追記は必要です。
      </div>
      <div>
        <strong>Q:</strong>撮影は本当に不要？<br>
        <strong>A:</strong>ベースはそろっていますが、オリジナル写真を追加したほうが効果的な場合もございます。
      </div>
      <div>
        <strong>Q:</strong>更新を放置しそうで不安…<br>
        <strong>A:</strong>簡単UIとサポートでフォローします。操作に不明点があれば気軽にお問い合わせください。
      </div>
    </div>
  </div>
</section>

<!-- CONTACT SECTION -->
<section class="contact-section">
  <div>
    <h2>お問い合わせ・無料相談</h2>
    <p class="mw-700">
      当サービスの導入や具体的な疑問点など、お気軽にご相談ください。<br>
      30日間お試しのプランもご用意しております。
    </p>
    <button>お問い合わせフォーム</button>
    <button>無料相談を予約する</button>
  </div>
</section>

<footer>
  <p>&copy; <span id="year"></span> Example Company. All Rights Reserved.</p>
  <p>運営会社: ○○株式会社 / 代表者: ○○ / 旧名称: インスタントホームページ / 特許番号: (もしあれば)</p>
  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</footer>

</body>
</html>
