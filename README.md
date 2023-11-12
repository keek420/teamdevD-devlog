# teamdevD-devlog

## 技術スタック

- 使用する言語　TypeScript
- 使用するフレームワーク（Vue、React など） Phaser
- 使用する CI (husky、github actions など）なし
- Linter とコードフォーマッターの設定（eslint、prettier など）なし

## タスク管理

- Trello(後日、設定 担当:COCO)

## ミーティング日程

- 水、土(金)  19:00~20:00


## 作るカードゲーム

- Blackjack

### 要件定義
- ブラウザで動く(extra 他のプラットフォーム)
- 最大４人でプレイ(まずは一人でプレイ用を開発)
    - 他のカードゲームや掛け金制度などの拡張性を念頭に開発


### ゲームの流れ

1. プレイヤーに二枚ずつ配られる
2. ディーラーのカードは一枚公開(プレイヤーにも公開、非公開は流用できるように)

3. プレイヤーのヒットorスタンド
    - ヒットの場合: デッキから一枚引いて手札に加える
    - スタンドの場合: 手札を確定
    - バーストの判定
4. スタンド or バストで手札確定

5. 3.4をプレイヤーごとに行う

6. ディーラは17以上になるまでカードを引く。
    バスト、バストしなかったプレイヤーは勝利、バストしたプレイヤーは負け
7. ディーラの手札を公開。点数が大きいプレイヤーは勝利(引き分けはプレイヤー負け)


## マイルストーン(スケジュール)
以下を目標として開発を行う

11/18 
Phaserの学習(勉強会)、要件定義、技術構成、ワイヤーフレーム、クラスアクティビティ

11/25 
(FE)基本画面、(BE)基本的なクラスの作成(カード、プレイヤー)

12/9  
ブラックジャック自体の完成(あくまでカードゲームとして遊べるくらい。)

12/23(最終)
  12/9時点の完成度によってTBD。他のゲームを作るか、拡張するか。
## deploy 環境を決める
- フロントエンドは Vercel
- バックエンドは Google Cloud Run、AWS、Render など（あとで）

## 難易度　
easy -  ディーラとの勝負
medium - 他プレイヤーとのスコアの競争、(cpu)
hard - 他プレイヤーとのスコアの競争、(cpu 頭いい)


# 議事録関係
- minutesに議事録を保存
