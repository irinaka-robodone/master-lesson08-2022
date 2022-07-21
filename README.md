# lesson08-2022-master

作成者: teacher
実施日: 07/21/2022

# 実装する機能

1. [x] micro:bit に文字表示
1. [x] 任意の位置でピクセル描画
1. [ ] プレイヤー位置の更新
1. [x] ボタンプッシュ検知
    - ゲーム開始用
    - バーの操作用
1. [ ] ボールの速度記録
1. [ ] 任意のボール位置でイベント発生させるロジック
1. [ ] スコアロジック
    - ゲームオーバー時に表示するスコア
    - スコアに応じてゲームの難易度を変化させる
    - 難易度の例はボールの速さ増加

# リモートで取り組む人は以下を読んで開発していこう！

1. マスタークラスのレッスンブック「レッスン８」をすべて目を通そう。
  - 今回は２回のレッスン（合計180分間）で micro:bit でピンポンゲームを制作します！
1. レッスンブックの内容に目を通せたら、まず 15 分でピンポンゲームで実装する機能を考えてリストアップしよう。
  - レッスンブック「レッスン８」の主な機能のページと以下のピンポンゲームのプレイ動画を参考に実装する機能を考えてリストアップする。
    - https://www.youtube.com/watch?v=BJ520s79cnM
    - https://www.youtube.com/watch?v=BDIrYfzlULE
  - このとき、必ず紙などに書いてリストアップすること。
  - この作業はコードを書き始める前、最初に必ずやること。アプリやサービスを開発することになったとき開発者が最初にやることが、この「要件定義」「機能設計」です。
  - 先生が行った要件定義は上の「実装する機能」に書いているよ。
1. コーディング
    - 自分がリストアップした機能を１つずつ実装していこう。
    - 先生の例だと、まず実装することになるのは「ボタンAを押したらゲームスタートする機能」になるね。
    - 
  
1. 「micro:bit 文法集」をどっちも見て
"""
while not button_a.was_pressed():
  pass
display.scroll('Game Start!')

IsGameOver = False # ゲームオーバー判定用の真偽値

while not IsGameOver: # IsGameOver が True になると while False になってループ終了する
  display.set_pixel(3, 3, 9)
  
  sleep(10) # 10ms ごとに画面の描画を更新する
  display.clear() #画面の描画をリセットする
