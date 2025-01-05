<!--
  Filename: top-page-wireframe.html
  Description: A single HTML file representing a wireframe for the Top Page
  Note: This wireframe is meant for demonstration. Please adjust styles, colors, images, and links as needed.
  You can copy-paste this entire code into your GitHub repository in one go.
-->

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Top Page Wireframe - "コンプリエイト（仮）" Example</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <!-- Minimal inline styling for wireframe visualization -->
  <style>
    * {
      box-sizing: border-box;
      margin: 0; 
      padding: 0;
      font-family: sans-serif;
    }
    body {
      background: #f9f9f9;
      color: #333;
      line-height: 1.4;
    }
    header, nav, footer, section, article {
      width: 100%;
      margin: 0 auto;
      max-width: 1200px;
      padding: 20px;
    }
    header, footer {
      background: #f0f0f0;
    }
    h1, h2, h3, h4 {
      margin-bottom: 10px;
      font-weight: normal;
    }
    a, button {
      cursor: pointer;
    }
    .container {
      margin: 0 auto;
      max-width: 1200px;
      padding: 20px;
    }
    .hero {
      background: #e6f1ff; /* Example background color for hero section */
      padding: 60px 20px;
      text-align: center;
    }
    .hero h1 {
      font-size: 2rem;
      margin-bottom: 16px;
    }
    .hero p {
      font-size: 1.1rem;
      margin-bottom: 24px;
      color: #444;
    }
    .hero .cta-buttons {
      display: inline-flex;
      gap: 10px;
      flex-wrap: wrap;
    }
    .cta-buttons a, .cta-buttons button {
      text-decoration: none;
      background: #0078ff; 
      color: #fff;
      padding: 12px 20px;
      border-radius: 4px;
      font-size: 1rem;
      border: none;
    }
    .features, .steps, .pricing, .faq, .contact-section {
      background: #fff;
      margin: 20px auto;
      padding: 20px;
      border-radius: 6px;
      box-shadow: 0 0 4px rgba(0,0,0,0.05);
    }
    .features h2, .steps h2, .pricing h2, .faq h2, .contact-section h2 {
      margin-bottom: 10px;
    }
    .features-list, .steps-list, .pricing-details, .faq-list {
      margin-top: 10px;
    }
    .features-list > div, 
    .steps-list > div, 
    .pricing-details > div, 
    .faq-list > div {
      margin-bottom: 16px;
    }
    /* Example minimal style for tables */
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
      color: #0078ff; /* Example highlight color */
      font-weight: bold;
    }
    /* Footer styles */
    footer {
      text-align: center;
      background: #fafafa;
      margin-top: 20px;
      padding: 30px;
      font-size: 0.9rem;
    }
    footer p {
      margin: 5px 0;
    }
    .mw-700 {
      max-width: 700px;
      margin: 0 auto;
    }
  </style>
</head>
<body>

<!-- HEADER / NAV -->
<header>
  <nav>
    <h2>コンプリエイトホームページ（仮）</h2>
    <!-- Possible navigation links, if needed -->
    <!-- <ul>
      <li><a href="#">トップ</a></li>
      <li><a href="#">料金</a></li>
      <li><a href="#">機能</a></li>
      <li><a href="#">サポート</a></li>
      <li><a href="#">お問い合わせ</a></li>
    </ul> -->
  </nav>
</header>

<!-- HERO SECTION -->
<section class="hero">
  <h1>写真や文章準備の負担を大きく軽減<br>あなたのホームページをすばやく整えます</h1>
  <p>
    業種に合った写真や例文を多数ご用意。<br>
    難しい操作や専門知識がなくても形になるから、本業に集中できます。
  </p>
  <div class="cta-buttons">
    <a href="#" onclick="alert('無料で相談ボタン クリック');">無料で相談してみる</a>
    <a href="#" onclick="alert('お試しボタン クリック');">30日お試しはこちら</a>
  </div>
</section>

<!-- FEATURES / CONCEPT SECTION -->
<section class="features">
  <h2>なぜ「手間を大幅に減らせる」のか？</h2>
  <div class="features-list">
    <div>
      <h3>1. 豊富な写真＆文章サンプル</h3>
      <p>
        業種別のイメージ写真や例文を多数取りそろえています。<br>
        ゼロからすべて用意する必要はなく、最低限の調整だけでサイトを整えられます。
      </p>
    </div>
    <div>
      <h3>2. 更新しやすい管理画面</h3>
      <p>
        専門知識のない方でも操作しやすいUIを採用。<br>
        定期的な写真差し替えや文章の追加・修正も、素早く完了します。
      </p>
    </div>
    <div>
      <h3>3. 特許取得の仕組みで検索リスクを軽減</h3>
      <p>
        共有コンテンツをみんなで使っても重複ペナルティのリスクを最小化。<br>
        月額費用にはこのシステム維持費も含まれています。
      </p>
    </div>
  </div>
</section>

<!-- STEPS SECTION -->
<section class="steps">
  <h2>サイト公開までの流れ</h2>
  <div class="steps-list">
    <div>
      <h4>ステップ1：基本情報を入力</h4>
      <p>事業内容や希望する業種など、簡単な初期設定だけ。</p>
    </div>
    <div>
      <h4>ステップ2：写真・例文を選ぶ</h4>
      <p>当社が保有する豊富なサンプルから合いそうなものをピックアップ。<br>
         必要があればご自身で追加の写真をアップロードしてOK。</p>
    </div>
    <div>
      <h4>ステップ3：独自の情報を少し追記</h4>
      <p>社名や店舗情報、料金メニューなど最低限の部分だけ修正すれば形が整います。</p>
    </div>
    <div>
      <h4>ステップ4：公開ボタンで完成</h4>
      <p>調整次第で数日程度でサイトを公開可能。少しずつカスタマイズして仕上げることもできます。</p>
    </div>
  </div>
</section>

<!-- PRICING SECTION -->
<section class="pricing">
  <h2>料金プラン</h2>
  <div class="pricing-details">
    <div>
      <strong>初期費用：59,800円</strong><br>
      <span>業種別写真・例文などのご利用開始に伴う費用。<br>
      一から撮影・ライティングを外注するより大幅に費用を抑えられます。</span>
    </div>
    <div>
      <strong>月額費用：5,980円</strong><br>
      <span>共有コンテンツシステムの維持費や特許取得の仕組み運用、基本サポートが含まれます。</span>
    </div>

    <!-- Comparison Table Example -->
    <table class="compare-table">
      <thead>
        <tr>
          <th></th>
          <th>DIYノーコード</th>
          <th>フルオーダー制作</th>
          <th><span class="highlight">コンプリエイト</span></th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>初期コスト</th>
          <td>低〜無料<br>(自力撮影・執筆が必要)</td>
          <td>数十万円〜<br>(撮影費やライティング費用別)</td>
          <td>59,800円<br>(写真＆例文利用開始費)</td>
        </tr>
        <tr>
          <th>更新コスト</th>
          <td>自力学習<br>時間も手間も自己負担</td>
          <td>更新の都度費用<br>制作会社に依頼</td>
          <td>月5,980円<br>(システム&サポート含む)</td>
        </tr>
        <tr>
          <th>撮影・文章作成</th>
          <td>すべて自前</td>
          <td>プロに依頼し予算増</td>
          <td>多くをサンプルで補完<br>必要なら独自分を追加可能</td>
        </tr>
      </tbody>
    </table>
  </div>
</section>

<!-- POSSIBLE "USE CASES" OR "INDUSTRIES" SECTION -->
<section class="features">
  <h2>こんな業種・目的におすすめ</h2>
  <div class="features-list">
    <div>
      <h3>美容サロン</h3>
      <p>季節のスタイルやキャンペーン写真の更新が手早く行えます。</p>
    </div>
    <div>
      <h3>建築・リフォーム</h3>
      <p>施工事例の写真をベース素材と組み合わせ、ビフォアーアフターの掲載もラクに。</p>
    </div>
    <div>
      <h3>不動産</h3>
      <p>物件写真の雛形を使って魅力的に紹介。<br>
         将来的に物件登録システムの開発も検討中です。</p>
    </div>
    <!-- ... More examples as needed -->
  </div>
  <p style="margin-top:20px;">
    上記以外にも、多くの業種に対応。<br>
    大がかりな原稿や撮影に時間をかけにくい小規模事業者の方に向いています。
  </p>
</section>

<!-- FAQ & SUPPORT -->
<section class="faq">
  <h2>よくある質問</h2>
  <div class="faq-list">
    <div>
      <strong>Q:</strong> 写真や文章がすべて揃っているって本当？<br>
      <strong>A:</strong> 多数の業種向け素材をご用意しています。ただし、店舗名や独自情報など、最低限の追記は必要です。
    </div>
    <div>
      <strong>Q:</strong> すべて撮影しなくていいの？<br>
      <strong>A:</strong> 場合によってはオリジナル写真を追加いただくほうが効果的ですが、基本的な雰囲気作りには弊社の写真サンプルが活用できます。
    </div>
    <div>
      <strong>Q:</strong> 更新が苦手でまた放置しそう…<br>
      <strong>A:</strong> 簡単な管理画面とサポート体制でフォローします。操作に不安があればお気軽にご相談ください。
    </div>
  </div>
</section>

<!-- CONTACT SECTION -->
<section class="contact-section">
  <h2>お問い合わせ・無料相談</h2>
  <p class="mw-700">
    当サービスの導入や具体的な疑問点など、お気軽にご相談ください。<br>
    <em>30日間お試しプラン</em>もご用意しています。
  </p>
  <br>
  <button onclick="alert('お問い合わせフォームへ');">問い合わせフォーム</button>
  <button onclick="alert('無料相談予約');">無料相談を予約</button>
</section>

<!-- FOOTER -->
<footer>
  <p>Copyright &copy; 
    <span id="year"></span> 
    Example Company, All Rights Reserved.
  </p>
  <p>
    運営会社: ○○株式会社 / 代表: ○○ / 旧名称: インスタントホームページ / 特許番号: (もしあれば)
  </p>
  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</footer>

</body>
</html>

