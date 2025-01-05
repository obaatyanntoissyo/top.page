<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8" />
  <title>トップページワイヤーフレーム - 「コンプリエイト（仮）」例</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <!--
    ---------------------------------------------------------
     このHTMLは「文章の羅列」感を減らし、よりワイヤーフレーム
     らしいレイアウトを示すためのコード例です。

     ・画像の代わりにグレー枠やイラスト風のプレースホルダーを表示
     ・トップページの要素をわかりやすく配置
     ・最小限のスタイルをあてて "箱" の位置が視覚化される
    ---------------------------------------------------------
  -->
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: sans-serif;
    }
    body {
      background: #fafafa;
      color: #333;
      line-height: 1.5;
    }
    header, nav, footer, section {
      width: 100%;
      max-width: 1100px;
      margin: 0 auto;
      padding: 20px;
    }

    /* ヘッダー全般 */
    header {
      background: #f0f0f0;
      margin-bottom: 20px;
    }
    header h1 {
      font-size: 1.4rem;
      margin-bottom: 5px;
    }

    /* ヒーローセクション */
    .hero {
      background: #d9ebff;
      margin-bottom: 20px;
      padding: 40px 20px;
      border-radius: 6px;
      text-align: center;
      position: relative;
    }
    .hero .hero-image-placeholder {
      width: 100%;
      max-width: 600px;
      height: 200px;
      background: repeating-linear-gradient(
        45deg,
        #ccc 0,
        #ccc 5px,
        #eee 5px,
        #eee 10px
      );
      margin: 0 auto 20px;
      border-radius: 4px;
    }
    .hero h2 {
      font-size: 1.6rem;
      margin-bottom: 10px;
      font-weight: bold;
    }
    .hero p {
      margin-bottom: 20px;
    }
    .hero .cta-buttons {
      display: inline-flex;
      gap: 10px;
      flex-wrap: wrap;
      justify-content: center;
    }
    .cta-buttons a, .cta-buttons button {
      background: #0078ff;
      color: #fff;
      text-decoration: none;
      padding: 12px 20px;
      border-radius: 4px;
      border: none;
      font-size: 1rem;
      transition: background 0.2s ease;
    }
    .cta-buttons a:hover, .cta-buttons button:hover {
      background: #005dc1;
    }

    /* 特徴セクション (Features) */
    .features {
      background: #fff;
      margin-bottom: 20px;
      border-radius: 6px;
      box-shadow: 0 0 4px rgba(0,0,0,0.05);
      padding: 20px;
    }
    .features h2 {
      margin-bottom: 10px;
      font-size: 1.3rem;
      font-weight: bold;
    }
    .feature-list {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      margin-top: 15px;
    }
    .feature-item {
      flex: 1 1 200px;
      min-width: 200px;
      background: #f7f7f7;
      padding: 15px;
      border-radius: 4px;
    }
    .feature-item h3 {
      font-size: 1.1rem;
      margin-bottom: 6px;
      color: #0078ff;
      font-weight: normal;
    }

    /* ステップセクション */
    .steps {
      background: #fff;
      margin-bottom: 20px;
      border-radius: 6px;
      box-shadow: 0 0 4px rgba(0,0,0,0.05);
      padding: 20px;
    }
    .steps h2 {
      font-size: 1.3rem;
      font-weight: bold;
      margin-bottom: 10px;
    }
    .step-list {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      margin-top: 10px;
    }
    .step-item {
      flex: 1 1 220px;
      min-width: 220px;
      background: #f7f7f7;
      padding: 15px;
      border-radius: 4px;
    }
    .step-item h4 {
      font-size: 1rem;
      margin-bottom: 6px;
      color: #0078ff;
      font-weight: bold;
    }

    /* 料金セクション */
    .pricing {
      background: #fff;
      margin-bottom: 20px;
      border-radius: 6px;
      box-shadow: 0 0 4px rgba(0,0,0,0.05);
      padding: 20px;
    }
    .pricing h2 {
      margin-bottom: 10px;
      font-size: 1.3rem;
      font-weight: bold;
    }
    .pricing .inner {
      margin-top: 10px;
    }
    .pricing-highlight {
      background: #eef;
      padding: 10px;
      border-radius: 4px;
      margin-bottom: 20px;
    }
    .compare-table {
      margin-top: 20px;
      border-collapse: collapse;
      width: 100%;
      background: #fafafa;
    }
    .compare-table th, .compare-table td {
      border: 1px solid #ccc;
      padding: 12px;
      text-align: left;
    }
    .highlight {
      color: #0078ff; 
      font-weight: bold;
    }

    /* おすすめ業種セクション */
    .industries {
      background: #fff;
      margin-bottom: 20px;
      border-radius: 6px;
      box-shadow: 0 0 4px rgba(0,0,0,0.05);
      padding: 20px;
    }
    .industries h2 {
      margin-bottom: 10px;
      font-size: 1.3rem;
      font-weight: bold;
    }
    .industry-list {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      margin-top: 10px;
    }
    .industry-item {
      flex: 1 1 220px;
      min-width: 220px;
      background: #f7f7f7;
      border-radius: 4px;
      padding: 15px;
    }
    .industry-item h3 {
      margin-bottom: 4px;
      color: #0078ff;
      font-weight: normal;
      font-size: 1.1rem;
    }

    /* FAQセクション */
    .faq-section {
      background: #fff;
      margin-bottom: 20px;
      border-radius: 6px;
      box-shadow: 0 0 4px rgba(0,0,0,0.05);
      padding: 20px;
    }
    .faq-section h2 {
      margin-bottom: 10px;
      font-size: 1.3rem;
      font-weight: bold;
    }
    .faq-list > div {
      margin-bottom: 16px;
    }
    .faq-list strong {
      color: #0078ff;
    }

    /* お問い合わせ */
    .contact-section {
      background: #fff;
      margin-bottom: 20px;
      border-radius: 6px;
      box-shadow: 0 0 4px rgba(0,0,0,0.05);
      padding: 20px;
      text-align: center;
    }
    .contact-section h2 {
      font-size: 1.3rem;
      font-weight: bold;
      margin-bottom: 15px;
    }
    .contact-section .btn {
      background: #0078ff;
      color: #fff;
      border: none;
      padding: 10px 18px;
      border-radius: 4px;
      margin: 8px;
      cursor: pointer;
      font-size: 1rem;
    }
    .btn:hover {
      background: #005dc1;
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
      margin: 6px 0;
    }
  </style>
</head>
<body>

<header>
  <h1>コンプリエイトホームページ（仮）</h1>
</header>

<!-- ヒーローセクション -->
<section class="hero">
  <!-- 画像やビジュアルのプレースホルダー -->
  <div class="hero-image-placeholder">
    <!-- グレーの繰り返しパターン背景などで実際にはイメージを差し込む位置 -->
  </div>
  <h2>写真や文章の下準備を大幅に軽減。<br>ホームページ作りで困らない。</h2>
  <p>
    多彩な業種向けの素材を備えているから、<br>
    初めてでもスムーズにサイトを整えられます。
  </p>
  <div class="cta-buttons">
    <a href="#">無料で相談する</a>
    <a href="#">30日間お試し</a>
  </div>
</section>

<!-- FEATURES -->
<section class="features">
  <h2>なぜ「手間を大幅に減らせる」の？</h2>
  <div class="feature-list">
    <div class="feature-item">
      <h3>1. 豊富な写真＆文章サンプル</h3>
      <p>
        業種別イメージや例文が揃っているので、<br>
        すべてを自分で作らなくてもOK。必要最低限のカスタマイズで形にできます。
      </p>
    </div>
    <div class="feature-item">
      <h3>2. 更新がラクラク</h3>
      <p>
        特別な操作スキルを要さずに写真や文面を差し替え可能。<br>
        放置リニューアルにも向いています。
      </p>
    </div>
    <div class="feature-item">
      <h3>3. 特許取得の仕組み</h3>
      <p>
        共有コンテンツを使っても重複ペナルティを抑える<br>
        特許技術を活用し、月額費用で安心の運用ができます。
      </p>
    </div>
  </div>
</section>

<!-- STEPS -->
<section class="steps">
  <h2>サイト公開までの流れ</h2>
  <div class="step-list">
    <div class="step-item">
      <h4>ステップ1：基本情報を登録</h4>
      <p>事業内容や業種など、簡単に入力。</p>
    </div>
    <div class="step-item">
      <h4>ステップ2：写真＆例文を選択</h4>
      <p>当社が用意したサンプルから合うものを探し、必要に応じて加筆。</p>
    </div>
    <div class="step-item">
      <h4>ステップ3：独自情報を追加</h4>
      <p>店舗名やサービス情報など最小限を追記すればOK。</p>
    </div>
    <div class="step-item">
      <h4>ステップ4：公開ボタンで完了</h4>
      <p>調整次第で数日程度。後から少しずつカスタマイズしていけます。</p>
    </div>
  </div>
</section>

<!-- PRICING -->
<section class="pricing">
  <h2>料金プラン</h2>
  <div class="inner">
    <div class="pricing-highlight">
      <p><strong>初期費用：59,800円</strong> — 業種別写真・例文を活用開始するための費用</p>
      <p><strong>月額：5,980円</strong> — 共有コンテンツや特許システム維持費＋サポートを含む</p>
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
          <td>低〜無料<br>(撮影・執筆は自作)</td>
          <td>数十万円〜<br>(撮影や原稿を制作会社へ依頼)</td>
          <td>59,800円<br>(写真&例文利用開始費用)</td>
        </tr>
        <tr>
          <th>更新コスト</th>
          <td>すべて自己作業<br>学習・手間大</td>
          <td>更新ごとに外注費用</td>
          <td>月5,980円<br>(特許システム&サポート込)</td>
        </tr>
        <tr>
          <th>写真・文章作成</th>
          <td>全て自前</td>
          <td>プロ依頼で予算大</td>
          <td>多くをサンプルで補填し、必要に応じオリジナル追加</td>
        </tr>
      </tbody>
    </table>
  </div>
</section>

<!-- INDUSTRIES EXAMPLES -->
<section class="industries">
  <h2>こんな業種・目的の方におすすめ</h2>
  <div class="industry-list">
    <div class="industry-item">
      <h3>美容サロン</h3>
      <p>新しいスタイル写真をすぐ反映、キャンペーン更新も楽々。</p>
    </div>
    <div class="industry-item">
      <h3>建築・リフォーム</h3>
      <p>施工事例をベース素材と合わせてビフォアーアフターを訴求。</p>
    </div>
    <div class="industry-item">
      <h3>不動産</h3>
      <p>物件写真の雛形で魅力を伝えやすい。<br>
         将来的に物件登録システム開発も検討中。</p>
    </div>
  </div>
  <p style="margin-top:20px;">
    その他の業種も多数対応。<br>
    お忙しい小規模企業の方に特におすすめです。
  </p>
</section>

<!-- FAQ SECTION -->
<section class="faq-section">
  <h2>よくある質問</h2>
  <div class="faq-list">
    <div>
      <strong>Q:</strong> 写真や文章は全く用意しなくていいんですか？<br>
      <strong>A:</strong> 業種向けの豊富な素材がありますが、店名や料金など独自情報は加筆いただく必要があります。
    </div>
    <div>
      <strong>Q:</strong> 撮影が苦手でも大丈夫？<br>
      <strong>A:</strong> ベースの写真があるので最低限の雰囲気は作れます。こだわりたい部分だけオリジナル写真を追加する方法がおすすめです。
    </div>
    <div>
      <strong>Q:</strong> 更新を放置してしまいそう…<br>
      <strong>A:</strong> 簡易UIとサポートで定期的な差し替えもスムーズ。操作に不安があればいつでもご連絡ください。
    </div>
  </div>
</section>

<!-- CONTACT SECTION -->
<section class="contact-section">
  <h2>お問い合わせ・無料相談</h2>
  <p>
    サービス導入に関する疑問や詳細をお聞きになりたい方は、<br>
    ぜひ下記よりご連絡ください。30日間お試しもご利用いただけます。
  </p>
  <button class="btn">お問い合わせフォーム</button>
  <button class="btn">無料相談を予約</button>
</section>

<!-- FOOTER -->
<footer>
  <p id="copyright">
    &copy; <span id="year"></span> Example Company. All Rights Reserved.
  </p>
  <p>運営会社: ○○株式会社 / 代表者: ○○ / 旧名称: インスタントホームページ / 特許番号: (もしあれば)</p>
  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</footer>

</body>
</html>
