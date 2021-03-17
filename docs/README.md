# 職務経歴書

<div style="text-align: right;">2021/03/17 現在</div>

<div style="text-align: right;">氏名 大橋芳生</div>

## 職務概要

<div style="border: 1px solid; margin: 1px;">
大学を卒業後、情報通信系開発会社に入社。一貫して物流業界の業務システム開発に携わる。1社目ではシステムエンジニアとしてプログラム基本設計から設計、開発を担当。2社目ではゼロからのスクラッチ開発を経験するため、ベンチャー企業に2年ほど在籍。企画、設計から開発業務、ときにはIT講師として幅広い経験を積む。現在は個人事業主として独立をし、先進的なマイクロサービスで多彩な言語の開発業務を経験。
</div>

## 職務経歴

<div style="display: flex; justify-content: space-between;">
  <div>個人事業主として活動</div>
  <div>(勤務期間: 2019/04 ~ 現在)</div>
</div>

## 基本情報

|key|value|
|---|-----|
|名前|<ruby><rb>大橋 芳生<rb><rt>おおはし よしき</rt></ruby>|
|生年月日|1993/04/28|
|ブログ|[tech-blog.yoshikiohashi.dev](https://tech-blog.yoshikiohashi.dev/)|
|ポートフォリオ|[yoshikiohashi.dev](https://yoshikiohashi.dev/)|
|GitHub|[yoshiki-0428](https://github.com/yoshiki-0428)|
|Twitter|[@yoshiki__0428](https://twitter.com/yoshiki__0428)|

## 学歴

- 2012年4月 ~ 2016年3月  
  - 新潟国際情報大学 情報システム学科

- 2009年4月 ~ 2012年3月
  - 新潟県立三条商業高等学校 商業科

## スキル

### 言語

- 日本語
  - ネイティブ
- 英語
  - 学生時代に2ヶ月ほど留学経験あり
  - 海外旅行で困らない程度の日常会話レベル
  - チャット上で国外エンジニアと仕様確認ができる

### プログラミング言語

- Java8, Java11
- Kotlin
- Go
- JavaScript
- TypeScript

### フレームワーク

- Spring
  - SpringBoot
  - Spring MVC
  - Spring WebFlux
  - Spring Security
  - Spring Cloud Gateway
- Golang
  - gin
  - echo
- Vue.js
- React.js
- Gatsby.js ([個人開発 | Gatsby Theme開発](https://github.com/yoshiki-0428/gatsby-all-pack-theme-starter))
- Next.js ([個人開発 | みんなのサブスク](https://review.subsc.cc/))
- frourio (個人開発)

### CI/CD

- GitHub Actions
- Circle CI
- GitLab CI

### その他周辺ツール

- OpenAPI Generator

## 職務経歴

### 2020/11 - 現在 : 株式会社コルデコ

|key|value|
|---|-----|
|職種|フロントエンドエンジニア|
|雇用形態|業務委託|
|事業内容|情報通信業|
|従業員数|15人以上|

#### CtoC DIY商品販売ECサイト開発

- **プロジェクト概要:**
  - サービス立ち上げ途中における機能強化を目的とした開発

- **プロジェクト規模:**
  - 15人
    - PM兼デザイナー: 3人
    - フロントエンド: 6人
    - バックエンド: 6人

- **役割:**
  - 機能検討、設計、コーディング、レビュー

- **プロジェクト詳細:**
  - React, TypeScript によるフロントエンド機能開発
  - Atomic Designを使用したエコシステムの構築
  - Cypressを利用したE2Eテスト環境の構築
  - GitHub Actionsを利用しE2E自動テスト環境の構築

- **利用技術:**
  - React.js(TypeScript), Redux, styled-components, Cypress, Jest
  - Golang (echo) ※一部API部分を担当
  - GitHub Actions

---

### 2019/10 - 2020/10 : 株式会社OPTiM

|key|value|
|---|-----|
|職種|Webアプリケーションエンジニア|
|雇用形態|業務委託|
|事業内容|IoTプラットフォーム開発事業者|
|従業員数|200名以上|

#### 手術ロボットリアルタイム監視ダッシュボード開発

- **プロジェクト概要:**
  - ゼロからのサービス立ち上げ
  - マイクロサービスアーキテクチャで構成されており、医療機器(IoT)からPOSTされるレコードをPubSubAPIでDBに保存をし、保存されたデータをリアルタイムにダッシュボードに表示させ、医療従事者に医療現場のログを可視化する価値を提供するシステム開発。

- **プロジェクト規模:**
  - 11人
    - IoTチーム: 2人
    - PM: 1人
    - インフラ: 1人
    - バックエンド: 3人
    - フロントエンド: 4人

- **役割:**
  - 機能検討(インセプションデッキ作成・検討)、設計、コーディング、レビュー

- **プロジェクト詳細:**
  - API
    - アプリの認証部分(OAuth2)を担当しました。Spring Cloud Gatewayを使用し、認証情報をGatewayに管理をさせ、フロントとFBBと通信を行うように処理をしました。実装方針としてはなるべくSpringの機能を最大限活用し、自分でコードは書かないことを意識しておりました。（FW内のコードで何をしているか理解し、必要な部分を置き換えることを重点的に行いました）

  - Front
    - Atomic Designの思想でコンポーネント開発を行いました。BFFとOAuth2認証、PubSubAPIでのリアルタイムデータ表示、Three.jsでのリアルタイムモデル再生といった先進的な技術挑戦をしました。

  - 詳細な技術解決内容は[こちら](https://job-draft.jp/users/45995#resume-header)に記載しております

- **利用技術:**
  - Golang, Java11, OpenAPI Generator, Spring WebFlux, Spring Boot, Spring Cloud Gateway, Jooq
  - Vue.js (TypeScript), Jest, Atomic Design
  - GitLab CI/CD

---

### 2019/04 - 2019/10 : GMOインターネット株式会社

|key|value|
|---|-----|
|職種|バックエンドエンジニア|
|雇用形態|業務委託|
|事業内容|情報通信業|
|従業員数|6000名以上|

#### 蓄電システムのWeb管理アプリケーション開発

- **プロジェクト概要:**
  - 既存システムの改修案件に携わりました。蓄電システムのWeb管理アプリのPM兼開発者として要件定義-結合フェーズまで担当

- **プロジェクト規模:**
  - ４人
    - PM兼開発: 1人
    - フロント: 2人
    - バックエンド: 1人

- **役割:**
  - 顧客機能提案、設計、コーディング、レビュー

- **プロジェクト詳細:**
  - SpringBootを使用したサーバーサイドAPI改修
  - フロントの画面開発
  - バッチ処理の改修（Shell Script）
  - 既存システムにDB Migrate
  - 空き時間に改善した内容
    - チームにIntelliJ IDEA導入
    - ローカル開発DB構築にDockerの導入
    - Seleniumを使用した自動テストの導入

- **利用技術:**
  - Java8, SpringBoot, thmeleaf, MyBatis
  - jQuery, Selenium
  - Docker, Flyway

---

### 2017/04 - 2019/03 :  株式会社クロノス

|key|value|
|---|-----|
|職種|Webアプリケーションエンジニア|
|雇用形態|正社員|
|事業内容|情報通信業|
|従業員数|200名以上|

#### 2018/06 - 2019/04 パチンコ・パチスロ情報統合アプリ開発

- **プロジェクト概要:**
  - 公共賭博の店舗情報などを公開するスマホアプリのAndroid、iOSアプリの改修案件を担当いたしました。改修内容としては、単純にアプリの画面開発だけでなく、新機能の追加の際に必要となるAPI項目の洗出〜作成依頼、アプリ側の通信〜画面表示までを担当

- **プロジェクト規模:**
  - 3人程度のタスクベースのアジャイル開発
    - PM: 1人
    - iOS: 1人
    - Android: 1人

- **役割:**
  - 画面設計、設計、コーディング、レビュー

- **プロジェクト詳細:**
  - 既存アプリのバグ改修や新規機能の追加業務を担当
  - APIチームへ開発に必要なJSONスキーマの連携
  - チーム内で振り返り手法のKPTを利用し、開発効率の向上
    - アプリ開発者からAPIチームへの連絡手段が限られる => 別チームにも気軽に連携できるように工夫

- **利用技術:**
  - Java(Android), 一部Kotlin, Objective-C
  - ButterKnife, PopInfo(通知系ライブラリ)
  - GitLab

#### 2018/01 - 2018/04 Slack, GmailをWatson APIに連携し社員モチベーションを管理するWebアプリケーション開発

- **プロジェクト概要:**
  - ゼロからの開発となりサービスの立ち上げを担当
  - 社員のモチベーションを外部GmailやSlack、その他チャットツールを利用し社員のモチベーションをWatsonAPIにより判定させるWebアプリケーション

- **プロジェクト規模:**
  - ４人
    - バックエンド: ２人 
    - フロントエンド: ２人 

- **役割:**
  - 画面設計、設計、コーディング、レビュー

- **プロジェクト詳細:**
  - Kotlin API, Vue.jsでのSPA開発
  - フロントからバックエンドにかけてCSVでのユーザ登録機能の作成

- **利用技術:**
  - Kotlin(SpringBoot), Gradle, MySQL, DOMA2
  - WatsonAPI, SlackAPI, ChatworkAPI
  - AWS EC2, Docker, docker-compose

#### 2017/09 - 2018/01 情報銀行PoCプロジェクト、旅行提案型Androidアプリ開発

- **プロジェクト概要:**
  - 情報銀行としての役割を試験的に検証するためのPoC案件
  - 登録者が詳細な個人情報以外の性格情報等を入力し、入力の代わりにオペレータなどが観光地の旅行プランを提案するAndroidアプリ

- **プロジェクト規模:**
  - PM: 1人
  - バックエンド: 1人
  - Android: 3人

- **役割:**
  - バックエンド設計、設計、コーディング、レビュー

- **プロジェクト詳細:**
  - Salesforceの基本設定、SalesforceのHeroku ConnectでのDB連携
  - Heroku Connect側のAPI設計

- **利用技術:**
  - Apex(Java), Salesforce, Heroku, Heroku Connect, SpringBoot
  - Java(Android)

> ※空白期間に関しては１ヶ月の短期間の社外研修業務を担当していたため記述を省略させていただいています。

#### 2017/04 - 2017/08 オリンピックマスコット募集サイト開発

- **プロジェクト概要:**
  - ゼロからの開発となりサービスの立ち上げを担当
  - 東京オリンピックのマスコットを募集するためのサイト

- **プロジェクト規模:**
  - 5人
    - PM: 1人
    - Salesforce構築＆画面開発: 1人
    - テスター: 3人

- **役割:**
  - 基本設計, 詳細設計、コーディング、レビュー

- **プロジェクト詳細:**
  - Salesforceのサイト公開機能を利用し公開ページを作成
  - 登録者に向けて仮登録機能、本登録機能、メール送信機能を提供
  - 仮登録時に有効期限を１時間としたtoken付きURLの発行
  - 複数画像の同時登録機能の提供

- **利用技術:**
  - Salesforce Site, Apex, Visualforce

---

### 2016/04 - 2017/3 : トリオシステムプランズ株式会社

|key|value|
|---|-----|
|職種|Webアプリケーションエンジニア|
|雇用形態|正社員|
|事業内容|情報通信業|
|従業員数|300名以上|


#### 2016/04 - 2017/03 大手スポーツメーカー物流システム開発 〜改修案件〜

- **プロジェクト概要:**
  - 海外流通のあるスポーツメーカーの内部システムの改修案件に携わる

- **プロジェクト規模:**
  - 10人
    - PM: 2人
    - エンジニア: 6人
    - テスター: 2人

- **役割:**
  - 設計、コーディング

- **プロジェクト詳細:**
  - SpringBootフレームワーク上でAPIの追加
  - 関税、国別通貨別の料金計算
  - 商品受注、料金計算を行うページの作成

- **利用技術:**
  - Java8, SpringBoot, thmyleaf, JPA
  - jQuery, JavaScript

---

## 課外活動

### 個人開発

* [みんなのサブスクメディアサイト企画・開発・運用](https://review.subsc.cc/)
* [Theme開発](https://github.com/yoshiki-0428/gatsby-all-pack-theme-starter)
* [ブログ作成](https://github.com/yoshiki-0428/engineer-blog)
* [ポートフォリオ作成](https://github.com/yoshiki-0428/vue_self_introdude)


## 副業

- 本の要約を各人で投稿できるCtoC Webサービスの開発
  - フォロワー２万人ほどいるマーケター、デザイナーと協力し現在開発中

- Web上でファイル編集・デザイン編集ができるWebツールの開発
  - 時給3000円ほどで契約し２ヶ月ほどフロントエンドエンジニアとして尽力
  
---

## 技術記事投稿

- Qiita
  - https://qiita.com/yoshiki-0428
- Blog
  - https://tech-blog.yoshikiohashi.dev/
- Zenn
  - https://zenn.dev/yoshiki__0428

---


## 意欲・興味

- チームで小さく早くリリースを行い、ユーザフィードバックを受けながら改善のサイクルを行う開発スタイルを好みます
- ユーザファーストでユーザインタビュー、インセプションデッキを行ってからプロダクト開発をするのが得意です
- 比較的バックエンドの実装が得意ですが、フロントエンドの実装も同等に可能です。インフラ構築経験がないため弱みと認識しています
- 一部テスト用CIを回したり、アプリレベルのDockerイメージビルドの構築が可能です
- リモートワークにおけるコミュニケーションの解決策としてペアプロ・モブプロを行い、ビジネスロジックの共有・チーム間の技術の継承を可能な限り行っています


