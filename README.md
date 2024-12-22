# ローグライクこうかとん

## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
* 主人公キャラクターこうかとんが探索するゲーム
* 9×9の迷路上のマップを自動生成しローグライク要素を追加
* 敵マスにプレイヤーが到達するとターン制の戦闘が開始
* マップを作成し一つのマップをクリヤすると次のマップへ
* マップ内にはプレイヤーのスキルを強化したり、新しいスキルを選択できる強化マス、プレイヤーhpを回復できる回復マス、敵が存在する敵マスを用意
* プレイヤーは最大でスキルを4つまで持てる
* マップを進むにつれて敵ガ強化される
* 画像の配布元URL: https://uzi-material.com/gallery-monster/

## ゲームの遊び方
* プレイヤーは十字キーでマップ内を移動
* 戦闘シーンではプレイヤーがスキルを選び行動する

## ゲームの実装
### 共通基本機能
* 背景画像と主人公キャラクターの描画

### 分担追加機能
* マップ自動生成（担当：イチカワ）：9×9の迷路となっているマップの自動生成
* 戦闘シーン（担当：コマイ）：プレイヤーと敵の戦闘
* bgm実装（担当：ノゲ）：探索フェイズや戦闘時のbgm実装
* キャラクター強化 (担当 :タイチ)　: プレイヤーの強化に関する関数
### ToDo
- [ ] プレイやーと敵の攻撃を実装
- [ ] 攻撃がプレイヤーや敵に当たった時の処理

### メモ
check_collisin関数で、ビームが壁の衝突判定を行う
distance関数で、敵とプレイヤーの距離を取得する
