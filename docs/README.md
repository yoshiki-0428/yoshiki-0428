# 職務経歴書

<div style="text-align: right;">2025/11/25 現在</div>

## 職務概要

<div style="border: 1px solid; padding: 3px;">
大学卒業後、ゼロからのスクラッチ開発を経験するため、ベンチャー企業に2年ほど在籍. 企画、設計から開発業務、ときにはIT講師として幅広い経験を積む. モダンな言語をスピード感早くキャッチアップするため個人事業主として約3年間経験し、先進的なマイクロサービスアーキテクチャで多彩な言語の開発業務を経験. その後、業務委託契約では「責任のある本番業務」が多く体験できないことを理由に正社員として楽天グループ株式会社に就職し. Ruby on Railsを用いたフリマアプリ開発で主に配送周りの新機能開発を担当. Yahoo! Japan株式会社に入社しマイクロサービス構成のECサイトの配送ドメインを担当. 知人の紹介でGovTech領域のパブリックテクノロジーズに入社. TLとして行政向けのAI領域の新規開発や公共交通の継続開発を担当しています. 

</div>

## 職務経歴

<!-- Pubtech Start -->

<div style="display: flex; justify-content: space-between; border-bottom: 1px solid; margin-top: 10px;">
    <div>株式会社パブリックテクノロジーズ - Public Technologies</div>
  <div>(勤務期間: 2024/07 ~ 現在)</div>
</div>

### 事業内容: 自治体向け公共ライドシェア、自治体職員向けLLMツールの提供等

<div class="career ">

| 期間 | 担当業務 | 開発環境等 | 役割/規模 |
| - | - | - | - |
| 2025/02<br>~<br>現在 | **自治体職員向けAI業務支援アプリの新規プロダクト開発**<br><br>自治体職員の方がNo Promptでステップ型のワークフローでLLMを簡単に利用できるAIサービスの新規開発にTech Leadとして技術選定・インフラ構築を取り組みました.<br><br>技術選定としてスピード感早く開発できる利点を得るため型安全でFEとOpenAPIでやり取りを行わないTypeScriptの型を共有できるtRPCを導入しました. また、TypeScriptの経験があれば気軽にBEも実装に着手できる技術者の学習コストの観点も考慮をしました. 構成はBE APIとFEを分けるベーシックな方式でIaC構築まで担当. 顧客から要望のあったIP制限もALBを用いてCloud Armorでの制御でスピード感早く対応をしました. <br>また、RAG検索のGCP VertexAI Searchを導入しスピーディに資料検索の機能を導入をし, GCPのDocumentAIを用いてLayout Parserで文書を意味理解できる状態でChunk化文章で学習処理を設計しました.<br>また、AIの機能開発ではLangChain, LangGraphによるLLM Workflowを構築したり、OpenAIだけでなく、Geminiでstreaming処理を開発しました. FEとの連携はSSEを採用し、JSONを都度都度送るのではなく、最小限のJSONを送信するように通信量を節約するように工夫をしました.<br>LLMOpsであるLangfuseをGCPにセルフホストするようにし、LLMのエラー監視、リランク処理も可能なように設計しました. 評価処理としてはOSSのRAGASを導入し, 回答の精度を自動評価できる仕組みづくりまでを設計しました.　<br>現在はDevOps的な立場となり、GHAを使用したGCP 1project内にBE(CloudRun)の複製環境を作成するなどし、PRのコンフリクト・衝突,staging相乗りデグレ問題解消,リリーススピード向上に貢献をしました. | tRPC / Fastify / TypeScript / Node.js<br>Nextjs<br>turborepo<br>Prisma<br>GCP CloudRun <br>Terraform<br>VertexAI Search<br>LG-WAN | エンジニア: 3人<br>デザイナー: 1人<br>PdM：1人 | </div> |
| 2024/10<br>~<br>2025/01 | **公共ライドシェアサービスの新機能開発**<br><br>当時、新しく提供予定だった香取市に固定路線バスで予約可能な新機能を開発しました. BEの開発が既にスタートしていたため, FEを担当しデザインとの繋込みを主に担当しました. <br>また, 負荷分散のためにライドシェアの配車計算処理のタスク処理を導入し自治体毎にCloud TaskのQueueで分散し、複数自治体導入したときに待ち時間を最小限にするようにしました. 配車計算は地域ごとに同時にはできなく、配車予定を計算の上決定されます. 今までは1processで稼働していた計算サーバを自治体別で計算できるように調整をしました. | Nextjs<br>OpenAPI/Swagger<br>Python/FastAPI<br>配車計算処理 (OR-Tools)<br>GCP Cloud Task / GCE | エンジニア: 2人<br>デザイナー: 1人<br>PdM：1人 |
| 2024/07<br>~<br>2024/09 | **3年間放置されたGCP環境のTerraform化**<br><br>入社当時、正社員エンジニアは自分だけだったため、数年間放置されたインフラを理解するためにも未経験だったTerraform（CDKの経験有）で既存リソースのIaC化を行いました。最初はGHAを利用し、CI/CD環境を構築したり、古き良きenvsルールで環境ごとにリソースを作成しました.<br>また、GHAからアプリケーションをデプロイできるようにGCP Workload Identityの設定で安全に秘匿情報をやり取りし、デプロイできる環境作成をしました.<br><br>後半からは、ブランチデプロイメントを実現するためにOSSのAtlantisサーバの導入をし、GitHub内でのコメントで複数環境をデプロイできるようにしました。これで1プロジェクトだけでなく、別のプロジェクトもGHAでTerraform CI/CDのコードを書くことなく、作業を標準化することにも貢献をしました. | Terraform<br>GCP<br>GitHub Actions | チーム規模 1人 |

<!-- Pubtech End -->


<!-- Yahoo Start -->

<div style="display: flex; justify-content: space-between; border-bottom: 1px solid; margin-top: 10px;">
    <div>LINEヤフー株式会社 - LY Corporation</div>
  <div>(勤務期間: 2023/01 ~ 2024/07)</div>
</div>

### 事業内容: 「PayPay」や「ヤフオク!」「Yahoo!ショッピング」などの100を超えるECサービスの開発・運用

<div class="career ">

| 期間 | 担当業務 | 開発環境等 | 役割/規模 |
| - | - | - | - |
| 2023/01<br>~<br>2024/06 | **Yahoo/ショッピング配送機能追加開発**<br><br>バックエンドエンジニアとして新配送機能の開発設計業務・リファクタ設計見積・リリース等の運用作業を担当<br><br>**範囲:** 要件定義、機能検討、設計、コーディング、レビュー<br><br>**詳細:**<br>マイクロサービス化された社内システムをもとに**3000rps**を超えるリクエストに耐えうる設計、アーキテクトを経験. 配送ドメインではJava11~18でAPI開発業務・仕様調整・スクラムで毎週見積もりで進める開発スタイルを取っている. | Java11, Java18<br>SpringBoot 3.0.1<br>Spring 5 WebFlux<br><br>社内クラウド<br>kubernetes<br> | チーム規模 8人<br><br>全体メンバー/400名~<br>Develop/200名<br>Businnes/200名<br> |

</div>

<!-- Yahoo End -->

<div style="display: flex; justify-content: space-between; border-bottom: 1px solid; margin-top: 10px;">
    <div>楽天グループ株式会社</div>
  <div>(勤務期間: 2021/06 ~ 2022/12)</div>
</div>


### 事業内容: Eコマース、フィンテック、デジタルコンテンツ、通信など７０以上のサービスの開発・運用

<div class="career ">

| 期間 | 担当業務 | 開発環境等 | 役割/規模 |
| - | - | - | - |
| 2021/06<br>~<br>2022/12 | **楽天/フリマアプリ追加機能開発**<br>バックエンドエンジニアとして新配送機能の開発設計業務・リファクタ設計見積<br><br>**範囲:** 要件定義、機能検討、設計、コーディング、レビュー<br><br>**詳細:**<br>ゆうパケットプラス・ポストに対応する設計・開発、コンビニ受取の設計・開発. 事業側との開発前のユーザストーリーマッピングを実施し, 開発の見える化に協力. チームの慣例に毎月のKPT振返りを主催し, 負担のかかっているエンジニアを見える化しました.<br>20億レコードを超えるテーブルにメンテナンスでカラム追加の実施. サマライズするクエリーのパフォーマンス・チューニングも担当<br>退職間際に着手した発送後のサイズ違い商品の金額が正しく取れていなかった問題を, 対抗のXML APIを利用してバッチ処理で料金を反映させる処理を追加, 安定的に変更をするためFeatureFlagを活用し, 年間約100~200万円程度の収益改善に貢献をしました.<br><br>その他アジャイル的取り組みとしてモブプロの定期開催・改善チーム参加・アプリケーション指向デザイン本輪読会開催など積極的に活動しました. | Ruby on Rails<br>一部Node.js<br><br>AWS EC2<br>Circle CI<br>GitHub Actions | メンバー/200名<br>Business/100名<br>Develop/100名 |

</div>

<div style="display: flex; justify-content: space-between; border-bottom: 1px solid; margin-top: 10px;">
    <div>個人事業主として活動</div>
  <div>(勤務期間: 2019/04 ~ 2021/05)</div>
</div>

### 事業内容: インターネットサービス開発・運営

<div class="career ">

| 期間 | 担当業務 | 開発環境等 | 役割/規模 |
| - | - | - | - |
| 2020/11<br>~<br>2021/05 | **DCM社/CtoC DIY商品販売ECサイト開発**<br>DIY商品のEC販売サイトの新規開発<br><br>**範囲:** 機能検討、設計、コーディング、レビュー<br><br>**詳細:**<br>フロントエンドエンジニアとして参画<br>React, TypeScript によるフロントエンド機能開発・認証部分も担当<br>Atomic Designを使用したエコシステムの構築<br>Cypressを利用したE2Eテスト環境の構築<br>GitHub Actionsを利用しE2E自動テスト環境の構築 | Golang(echo)<br><br>React(TypeScript)<br>Redux, styled-components, Cypress, Jest<br><br>GitHub Actions | メンバー/15名 |
| 2019/10<br>~<br>2020/10 | **(株)OPTiM/手術ロボットリアルタイム監視ダッシュボード開発**<br>マイクロサービスアーキテクチャで構成. 医療機器(IoT)からPOSTされるレコードをPubSubAPIでDBに保存をし、保存されたデータをリアルタイムにダッシュボードに表示させ、医療従事者に医療現場のログを可視化する価値を提供するシステム開発.<br><br>**範囲:** 機能検討(インセプションデッキ作成・検討)、設計、コーディング、レビュー<br>**API:** アプリの認証部分(OAuth2)を担当. Spring Cloud Gatewayを使用し、認証情報をGatewayに管理をさせ、フロントとFBBと通信を行うように処理をしました. 実装方針としてはなるべくSpringの機能を最大限活用（Springはエコシステム上最適と判断し選択）<br>**Front:** Atomic Designの思想でコンポーネント開発. BFF、OAuth2認証、WebSocket, SSEでのリアルタイムデータ表示、Three.jsでロボットリアルタイムモデル再生といった先進的な技術挑戦を経験.<br><br>詳細な技術解決内容は[こちら](https://job-draft.jp/users/45995#resume-header)に記載しております<br>（https://job-draft.jp/users/45995#resume-header） | Java11<br>Golang, OpenAPI<br>Spring WebFlux,<br>Spring Boot,<br>SpringCloudGateway, JOOQ<br><br>Vue.js, Jest, Atomic Design<br><br>GitLab CI/CD | メンバー/11名 |
| 2019/04<br>~<br>2019/09 | **GMO社/蓄電システム顧客管理Webアプリ**<br>既存システムの改修案件に携わる. 蓄電システムのWeb管理アプリのPM兼開発者として要件定義-結合フェーズまで担当<br><br>**範囲:** 顧客機能提案、設計、コーディング、レビュー<br><br>**詳細:**<br>SpringBootを使用したサーバーサイドAPI改修<br>フロントの画面開発<br>バッチ処理の改修（Shell Script）<br>既存システムDBにFlywayを導入<br>・空き時間に改善した内容<br>チームにIntelliJ IDEA導入, ローカル開発DB構築にDockerの導入, Seleniumを使用した自動テストの導入 | Java8, SpringBoot, Thymeleaf, MyBatis<br><br>jQuery, Selenium<br><br>Docker, Flyway<br> | PM/4人 |

</div>

<div style="display: flex; justify-content: space-between; border-bottom: 1px solid; margin-top: 10px;">
    <div>株式会社クロノス</div>
  <div>(勤務期間: 2017/04 ~ 2019/03)</div>
</div>

### 事業内容: AIソリューション、Web・モバイルアプリ開発、IT研修

<div class="career">

| 期間 | 担当業務（プロジェクト内容） | 開発環境等 | 役割/規模 |
| - | - | - | - |
| 2018/06<br>~<br>2019/03 | **DMM社/パチンコ・パチスロ情報統合アプリ開発**<br>公共賭博の店舗情報などを公開するスマホアプリのAndroid、iOSアプリの改修案件を担当いたしました. 改修内容としては、単純にアプリの画面開発だけでなく、新機能の追加の際に必要となるAPI項目の洗出〜作成依頼、アプリ側の通信〜画面表示までを担当<br><br>**範囲:** 画面設計、設計、コーディング、レビュー<br><br>**詳細:**<br>既存アプリのバグ改修や新規機能の追加業務を担当<br>APIチームへ開発に必要なJSONスキーマの連携<br>チーム内で振り返り手法のKPTを利用し、開発効率の向上<br>アプリ開発者からAPIチームへの連絡手段が限られる => 別チームにも気軽に連携できるように工夫 | Java(Android)<br>Kotlin<br>Objective-C<br>ButterKnife, PopInfo(通知ライブラリ)<br>GitLab | メンバー/3人 |
| 2018/01<br>~<br>2018/04 | **自社サービス／社員モチベーション管理Webアプリ**<br>ゼロからの開発となりサービスの立ち上げを担当<br>社員のモチベーションを外部GmailやSlack、その他チャットツールを利用し社員のモチベーションをWatsonAPIにより判定させるWebアプリケーション<br><br>**範囲:** 画面設計、設計、コーディング、レビュー<br><br>**詳細:**<br>Kotlin(Spring), Vue.jsでのSPA開発<br>SlackAPIとの認証処理<br>フロントからバックエンドにかけてCSVでのユーザ登録機能の作成 | Kotlin(Spring)<br>Gradle<br>MySQL, DOMA2<br><br>WatsonAPI, SlackAPI, ChatworkAPI<br><br>AWS EC2, Docker, docker-compose | メンバー/4人 |
| 2017/09<br>~<br>2018/01 | **情報銀行PoCプロジェクト、旅行提案型Androidアプリ開発**<br>情報銀行としての役割を試験的に検証するためのPoC案件<br>登録者が詳細な個人情報以外の性格情報等を入力し、入力の代わりにオペレータが観光地の旅行プランを提案するAndroidアプリ<br><br>**範囲:** バックエンド設計、設計、コーディング、レビュー<br><br>**詳細:** <br>Salesforceの基本設定、SalesforceのHeroku ConnectでのDB連携<br>Heroku Connect側のAPI設計 | Apex(Java) <br>Salesforce, Heroku, Heroku Connect, SpringBoot<br>Java(Android) | メンバー/5人 |
| 2017/04<br>~<br>2017/08 | **官公庁/オリンピックマスコット募集サイト開発**<br>ゼロからの開発となりサービスの立ち上げを担当<br>東京オリンピックのマスコットを募集するためのサイト<br><br>**範囲:** 基本設計, 詳細設計、コーディング、レビュー<br><br>**詳細:**<br>Salesforceのサイト公開機能を利用し公開ページを作成<br>登録者に向けて仮登録機能、本登録機能、メール送信機能を提供<br>仮登録時に有効期限を１時間としたtoken付きURLの発行<br>複数画像の同時登録機能の提供 | Salesforce Site, Apex, Visualforce | メンバー/5人 |

</div>
    
<div style="display: flex; justify-content: space-between; border-bottom: 1px solid; margin-top: 10px;">
    <div>トリオシステムプランズ株式会社</div>
  <div>(勤務期間: 2016/04 ~ 2017/03)</div>
</div>

### 事業内容: 製造、流通業、医療のシステム開発事業

<div class="career">

| 期間 | 担当業務（プロジェクト内容） | 開発環境等 | 役割/規模 |
| - | - | - | - |
| 2016/04<br>~<br>2017/03 | **YONEX/物流システム開発**<br>海外流通のあるスポーツメーカーの内部システムの改修案件に携わる<br><br>**範囲:** 設計、コーディング<br><br>**詳細:**<br>SpringBootフレームワーク上でAPIの追加<br>関税、国別通貨別の料金計算<br>商品受注、料金計算を行う画面開発 | Salesforce<br>Java8, SpringBoot<br>thymeleaf, JPA<br>jQuery, JavaScript | メンバー/5人 |

</div>

## スキル

| 種類 | 言語環境 | 期間 | レベル |
| - | - | - | - |
| **言語** | Java8, Java11 | ★4年 | メンバーに指導ができる |
|  | Kotlin | ★1年 | 業務で即戦力になれる |
|  | Golang | ★1年 | 業務で即戦力になれる |
|  | TypeScript | ★3年 | 業務で即戦力になれる |
| DB | MySQL | ★2年 | 構築からチューニングまで対応できる |
|  | PostgresSQL | ★1年 | 知識がある |
| フレームワーク | Spring Boot | ★3年 | メンバーに指導ができる |
|  | Spring MVC | ★1年 | メンバーに指導ができる |
|  | Spring WebFlux | ★1年 | メンバーに指導ができる |
|  | Spring Cloud Gateway | ★1年 | メンバーに指導ができる |
|  | Rails | ★2年 | 業務で即戦力になれる |
|  | Vue.js | ★2年 | メンバーに指導ができる |
|  | React.js | ★2年 | メンバーに指導ができる |
|  | Next.js (12, 13) | 2年 | 業務で即戦力になれる |
| **CI/CD** | GitHub Actions | ★1年 | 使用経験がある |
|  | AWS CodePipeline, CDK | ★1年 | 使用経験がある |
|  | GitLab CI | ★1年 | 使用経験がある |

> ※ 業務経験あり：★　

## 保有資格

- TOEIC 500 (2021/07/20)
- Oracle Java Silver SE 8
- 日商簿記検定3級
- 色彩検定2級

## 自己PR

　バックエンドからフロントエンドまで幅広く設計ができるWebアプリエンジニアです. 具体的な言語はGo, Java, Next.js, TypeScriptを使用し、各言語特性を理解しマイクロサービスなアーキテクチャでのアプリ設計が可能です. 
　バックエンド、OAuth2の認証部分の実装や、DBのSQLチューニング、BFFの構築をしフロントに連携して開発ができます. また、Spring5のWebFluxをコントロールし、PubSubAPIを通じたリアルタイムイベントの実装も担当いたしました.
　フロントエンド、AtomicDesignでのコンポーネント思想、通信部分と表現部分を分離して開発することの重要性を理解しております. また、Three.jsのWebGLとSSE（リアルタイムイベント）を使用したロボットモデルのリアルタイムモデル再生といった先進的な技術的挑戦も業務で担当いたしました.
アプリレイヤーだけでなく、各アプリのDockerイメージ化や、簡易スクリプトをk8s上でCronJob化するなど、アプリレイヤーからインフラ層へ繋げるスキルも持ち合わせております.

最近ではチームビルディングに興味があり、現在のチームで同じ課題を共有するためにYWT振返りをしたり、PJの機能見落としを防ぐためのユーザストーリーマッピング、ユースケースMTGをしています。

## 課外活動

### 技術投稿

- GitHub: https://github.com/yoshiki-0428
- Blog: https://tech-blog.yoshikiohashi.dev
- Qiita: https://qiita.com/yoshiki-0428

### 個人開発

- [Web地図アプリ開発 ねこまっぷ](https://nekomap.vercel.app)(https://nekomap.vercel.app)
- [みんなのサブスクメディアサイト企画・開発・運用](https://review.subsc.cc/)(https://review.subsc.cc/)
- [ブログ開発](https://github.com/yoshiki-0428/engineer-blog)(https://github.com/yoshiki-0428/engineer-blog)
- [Gatsby Theme開発](https://github.com/yoshiki-0428/gatsby-all-pack-theme-starter)(https://github.com/yoshiki-0428/gatsby-all-pack-theme-starter)
- [3Dモデルを活かしたポートフォリオ作成](https://github.com/yoshiki-0428/vue_self_introdude)(https://github.com/yoshiki-0428/vue_self_introdude)

### Side Job

- 医療系SaaSの開発お手伝い
  - Ruby on Railsでフルスタックに開発
  - AWS CDKを用いてCI/CD環境の構築
- Omusubi-chのBackend開発をお手伝い
  - コラボ配信のバックエンド設計・開発作業を担当
  - API: Golang Gin, DB: Dynamodb
- CtoCの本の要約サービスのアーキテクトを設計・開発〜リリース
  - Next.jsで開発 型、クライアント自動生成技術で開発作業を短縮
  - https://lecshire.com

## 興味・意欲

- チームで小さく早くリリースを行い、ユーザフィードバックを受けながら改善のサイクルを行う開発スタイルを好みます
- ユーザファーストでユーザインタビュー、インセプションデッキを行ってからプロダクト開発をするのが得意です
- 比較的バックエンドの実装が得意ですが、フロントエンドの実装も同等に可能です.インフラ構築経験がないため弱みと認識しています
- 一部テスト用CIを回したり、アプリレベルのDockerイメージビルドの構築が可能です
- リモートワークにおけるコミュニケーションの解決策としてペアプロ・モブプロを行い、ビジネスロジックの共有・チーム間の技術の継承を可能な限り行っています
