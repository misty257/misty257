## テトリス ##


### 設計 ###

テトリスのゲーム機能を以下3つに分類。

+ フィールドクラス
+ テトリミノクラス
+ ゲームクラス

### フィールドクラス ###

クラスの汎用的な機能・設定

+ フィールド(テトリス画面の作成)
+ 現在フィールド上にあるテトリミノを保持
+ 次以降に落下するテトリミノを保持
+ テトリミノの回転命令を受け付け、テトリミノが回転できる場合に回転
+ テトリミノの左右移動命令を受け付け、テトリミノが移動できる場合に移動
+ テトリミノの下移動命令を受け付け、テトリミノが移動できる場合に移動させ、移動できない場合はフィールドに固定
+ テトリミノの固定で行が全てブロックで埋まったら行を削除し、上にあるブロックを下に移動
+ 次のテトリミノをフィールドに設定、次以降に落下するテトリミノを生成
+ フィールドからはみ出したブロックがある場合はゲームオーバー

### テトリミノクラス ###

クラスの汎用的な機能・設定

+ テトリスブロックの作成(種類を定義)
+ ランダムにテトリミノを選択
+ テトリミノの回転処理

### ゲームクラス ###

クラスの汎用的な機能・設定

+ クラスの汎用的な機能・設定
+ 各操作受付制御
+ 自動落下処理
+ スコア、レベルの算出
+ テトリミノの固定から次のテトリミノ表示の制御
ゲームクラスではフィールドクラスが扱う機能以外を扱う感じ。

### ビュークラス ###






